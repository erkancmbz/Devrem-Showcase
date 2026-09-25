# 📚 Devrem Studio - Görsel Öğretici & Modül Kullanım Rehberi

> Bu rehber, **Devrem Studio (EEM Rehber)** platformunda yer alan tüm sanal laboratuvar araçlarının, mikrodenetleyici pinout sisteminin ve interaktif simülatörlerin nasıl kullanılacağını ekran görüntüleriyle adım adım açıklamaktadır.

---

## 📌 İçindekiler
1. [Ana Arayüz & Genel Bakış](#1-ana-arayüz--genel-bakış)
2. [Analog Filtre Tasarımı & Bode Eğrisi](#2-analog-filtre-tasarımı--bode-eğrisi)
3. [2. Derece Kontrol Sistemleri & Basamak Yanıtı](#3-2-derece-kontrol-sistemleri--basamak-yanıtı)
4. [Fazör Analizörü & Dinamik Vektör İzdüşümü](#4-fazör-analizörü--dinamik-vektör-izdüşümü)
5. [3-Fazlı Güç & Dengesiz Yük Simülatörü](#5-3-fazlı-güç--dengesiz-yük-simülatörü)
6. [Op-Amp 7 Devre Topolojisi & Kırpılma Osiloskobu](#6-op-amp-7-devre-topolojisi--kırpılma-osiloskobu)
7. [Web Audio Gerçek Zamanlı Sinyal Jeneratörü](#7-web-audio-gerçek-zamanlı-sinyal-jeneratörü)
8. [Smith Chart RF Empedans Eşleme](#8-smith-chart-rf-empedans-eşleme)
9. [İnteraktif Mikrodenetleyici (MCU) Pinout Rehberi](#9-interaktif-mikrodenetleyici-mcu-pinout-rehberi)
10. [KaTeX Matematiksel Formül Flashcard'ları](#10-katex-matematiksel-formül-flashcardları)

---

## 1. Ana Arayüz & Genel Bakış

Platform açıldığında sizi karşılayan ana çalışma istasyonu; modern **2026 Obsidian Gece Teması** ve **Pastel Gündüz Teması** seçenekleri, `Ctrl + K` hızlı arama çubuğu ve procedurally-generated (algoritmik çizilen) interaktif PCB arka planı ile donatılmıştır.

![Devrem Studio Ana Arayüz](images/overview/devrem_studio_hero.png)

* **Spotlight Arama (`Ctrl + K`):** Saniyeler içinde 15+ laboratuvar aracına, sınav sorularına veya formüllere doğrudan odaklanmanızı sağlar.
* **Akıllı Sınıf Filtresi:** 1-2. Sınıf (Temel Devreler), 3. Sınıf (Sinyal/Kontrol), 4. Sınıf (Bitirme/Uzmanlaşma) veya Kariyer moduna göre arayüzü filtreler.

---

## 2. Analog Filtre Tasarımı & Bode Eğrisi

Analog aktif ve pasif filtre devrelerinin frekans cevabını canlı olarak analiz eder.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![Bode Filtre Koyu](images/simulators/bode_filtre_koyu.png) | ![Bode Filtre Açık](images/simulators/bode_filtre_acik.png) |

### Nasıl Kullanılır?
1. Filtre tipini seçin: **Alçak Geçiren (LPF)**, **Yüksek Geçiren (HPF)**, **Bant Geçiren (BPF)** veya **Bant Durduran (Notch)**.
2. Direnç ($R$) ve Kondansatör ($C$) değerlerini girin.
3. Kanvas üzerinde farenizi gezdirdiğinizde:
   * Kesim frekansı ($f_c = \frac{1}{2\pi RC}$) anlık olarak işaretlenir.
   * İmlecin bulunduğu frekanstaki kazanç ($dB$) ve faz açısı ($\theta$) anlık yeşil HUD bilgi balonunda gösterilir.

---

## 3. 2. Derece Kontrol Sistemleri & Basamak Yanıtı

Kontrol mühendisliğinin temelini oluşturan 2. derece transfer fonksiyonlarının basamak tepkisini ($y(t)$) yüksek hassasiyetle simüle eder.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![Kontrol Sistemi Koyu](images/simulators/kontrol_sistemi_koyu.png) | ![Kontrol Sistemi Açık](images/simulators/kontrol_sistemi_acik.png) |

### Analiz Edilen Kritik Parametreler:
* **Sönüm Oranı ($\zeta$):**
  * $\zeta = 0$: Sönümsüz osilasyon
  * $0 < \zeta < 1$: Eksik sönümlü (aşım yapan dinamik yanıt)
  * $\zeta = 1$: Kritik sönümlü
  * $\zeta > 1$: Aşırı sönümlü
* **Doğal Frekans ($\omega_n$):** Sistemin tepki verme hızını belirler.
* **Grafik Üzerinde Canlı Okuma:** Tepe aşımı ($M_p$), oturma zamanı ($T_s \pm \%2$) ve yükselme zamanı ($T_r$) fare hareketine duyarlı olarak gösterilir.

---

## 4. Fazör Analizörü & Dinamik Vektör İzdüşümü

Alternatif akım (AC) devrelerinde karmaşık sayıları fazör oklarına dönüştürür.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![Fazör Koyu](images/simulators/fazor_analizi_koyu.png) | ![Fazör Açık](images/simulators/fazor_analizi_acik.png) |

### Özellikler:
* **Kutupsal & Kartezyen Giriş:** $V = V_{max} \angle \theta^\circ$ veya $V = a + jb$ formatında anında çift yönlü dönüşüm.
* **Canlı İzdüşüm:** Gerçek (Reel) ve Sanal (İmajiner) eksenlerdeki bileşenler, açı yayları ve genlik vektörü HiDPI kanvasta çizilir.

---

## 5. 3-Fazlı Güç & Dengesiz Yük Simülatörü

Endüstriyel güç sistemlerinde dengeli ve dengesiz 3 fazlı yükleri modeller.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![3 Faz Koyu](images/simulators/uc_faz_guc_koyu.png) | ![3 Faz Açık](images/simulators/uc_faz_guc_acik.png) |

* **Bağlantı Modları:** Yıldız ($Y$) ve Üçgen ($\Delta$) yük konfigürasyonları.
* **Nötr Akımı Analizi:** Dengesiz yüklerde nötr hattından ($I_N$) geçen artık akımın büyüklüğü ve faz açısı canlı hesaplanır.
* **Falstad Simülasyonu:** Tek tıkla ilgili devreyi tarayıcı içi Falstad simülatöründe çalıştırma bağlantısı.

---

## 6. Op-Amp 7 Devre Topolojisi & Kırpılma Osiloskobu

Operasyonel yükselteçlerde (LM741, TL072 vb.) giriş sinyali ile çıkış sinyalini karşılaştırmalı olarak osiloskopta gösterir.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![Op-Amp Koyu](images/simulators/opamp_osiloskop_koyu.png) | ![Op-Amp Açık](images/simulators/opamp_osiloskop_acik.png) |

* **Desteklenen 7 Topoloji:** Eviren (Inverting), Evirmeyen (Non-Inverting), Gerilim İzleyici (Buffer), Toplayıcı (Summing), Fark Alıcı (Difference), Türev Alıcı (Differentiator), İntegral Alıcı (Integrator).
* **Ray-Ray Doyum (Clipping):** Giriş sinyali besleme gerilimlerini ($\pm V_{cc}$) aştığında çıkışın nasıl düzleşip kırpıldığını gerçek zamanlı gösterir.

---

## 7. Web Audio Gerçek Zamanlı Sinyal Jeneratörü

Cihazınızın ses işlemcisini kullanarak laboratuvar tipi fonksiyon üreteci görevi görür.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![Sinyal Jeneratörü Koyu](images/simulators/sinyal_jeneratoru_koyu.png) | ![Sinyal Jeneratörü Açık](images/simulators/sinyal_jeneratoru_acik.png) |

* **Frekans Aralığı:** 20 Hz ile 20.000 Hz arası hassas kaydırıcı kontrolü.
* **Dalga Formları:** Sinüs, Kare, Üçgen, Testere Dişi.
* **Osiloskop Ekranı:** Üretilen ses sinyalinin zamana bağlı dalga formu doğrudan kanvas üzerinde çizilir.

---

## 8. Smith Chart RF Empedans Eşleme

RF, mikrodalga ve yüksek frekans iletim hatlarında empedans eşleme analizörü.

| Koyu Tema Görünümü | Açık Tema Görünümü |
| :---: | :---: |
| ![Smith Chart Koyu](images/simulators/smith_chart_koyu.png) | ![Smith Chart Açık](images/simulators/smith_chart_acik.png) |

* Sabit direnç ($r$) ve sabit reaktans ($x$) çemberleri üzerinde normalize yük empedansını ($z_L = r + jx$) konumlandırır.
* Yansıma katsayısı genliği ($|\Gamma|$), açısı ve Gerilim Duran Dalga Oranı (VSWR) anında hesaplanır.

---

## 9. İnteraktif Mikrodenetleyici (MCU) Pinout Rehberi

Gömülü sistem geliştiricileri için SVG tabanlı, tam etkileşimli pin şeması.

| Arduino Uno (Koyu) | Arduino Uno (Açık) |
| :---: | :---: |
| ![Arduino Uno Koyu](images/pinouts/arduino_uno_koyu.png) | ![Arduino Uno Açık](images/pinouts/arduino_uno_acik.png) |

### Çevresel Birim Filtreleme (PWM, I2C, SPI, UART, ADC)
Pencerelerdeki filtre butonlarına basıldığında (örneğin **PWM** seçildiğinde), ilgisiz tüm pinler soluklaşır ve yalnızca PWM destekleyen donanımsal pinler parlar:

![Arduino Uno PWM Filtresi](images/pinouts/arduino_uno_pwm_filtresi.png)

### Desteklenen Popüler Kartlar:
| ESP32 DevKit v1 | STM32 BlackPill (F401) | Raspberry Pi Pico (RP2040) |
| :---: | :---: | :---: |
| ![ESP32](images/pinouts/esp32_devkit_koyu.png) | ![STM32](images/pinouts/stm32_blackpill_koyu.png) | ![Pico](images/pinouts/raspberry_pi_pico_koyu.png) |

### Grafik ve Tablo Görünümü Geçişi
Geliştiriciler dilerse tek bir butonla görsel kart şemasından tüm pin alternatiflerinin listelendiği yüksek kontrastlı tablo moduna geçebilir:

![MCU Tablo Görünümü](images/pinouts/mcu_pinout_tablo_gorunumu.png)

---

## 10. KaTeX Matematiksel Formül Flashcard'ları

Sınavlara hazırlanan mühendislik öğrencileri için formül ezberleme ve soru-cevap kartları.

| Soru / Ön Yüz (Koyu) | Detaylı Çözüm / Arka Yüz (Koyu) |
| :---: | :---: |
| ![Flashcard Ön Koyu](images/flashcards/flashcard_on_yuz_koyu.png) | ![Flashcard Arka Koyu](images/flashcards/flashcard_arka_yuz_koyu.png) |

| Soru / Ön Yüz (Açık) | Detaylı Çözüm / Arka Yüz (Açık) |
| :---: | :---: |
| ![Flashcard Ön Açık](images/flashcards/flashcard_on_yuz_acik.png) | ![Flashcard Arka Açık](images/flashcards/flashcard_arka_yuz_acik.png) |

* **KaTeX LaTeX Render:** Laplace dönüşümleri, Maxwell denklemleri, Miller teoremi, Shannon kapasitesi ve rezonans formülleri kitap netliğinde matematiksel dizgiyle ekrana gelir.
* **Flip (Çevir) Animasyonu:** Karta tıklandığında yumuşak bir 3D dönüş efektiyle sorunun cevabı ve mühendislik yorumu açılır.

---

*Devrem Studio - Elektrik-Elektronik Mühendisliği Profesyonel Çalışma İstasyonu*
