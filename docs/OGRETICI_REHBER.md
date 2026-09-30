# 📚 Devrem Studio - Görsel Öğretici & Modül Kullanım Rehberi

> Bu rehber, **Devrem Studio (EEM Rehber)** platformunda yer alan tüm sanal laboratuvar araçlarının (27 mühendislik aracı), 8 yarıyıl / 240 AKTS Bologna müfredatının, mikrodenetleyici pinout sisteminin ve interaktif simülatörlerin nasıl kullanılacağını adım adım açıklamaktadır.

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
11. [8 Yarıyıl / 240 AKTS Bologna Müfredatı & Laboratuvar Köprüsü](#11-8-yarıyıl--240-akts-bologna-müfredatı--laboratuvar-köprüsü)
12. [Transformatör Eşdeğer Devre Simülatörü (P0)](#12-transformatör-eşdeğer-devre-simülatörü-p0)
13. [3-Faz Zikzak (Zn) & Vektör Saat Kadranı (P0)](#13-3-faz-zikzak-zn--vektör-saat-kadranı-p0)
14. [Güç Elektroniği DC-DC Dönüştürücü & 3-Kanal Osiloskop (P1)](#14-güç-elektroniği-dc-dc-dönüştürücü--3-kanal-osiloskop-p1)
15. [Asenkron Motor Tork-Hız & V/f Sürücü Lab (P1)](#15-asenkron-motor-tork-hız--vf-sürücü-lab-p1)
16. [Güç Sistemleri İletim Hattı, ABCD & Ferranti Etkisi (P1)](#16-güç-sistemleri-iletim-hattı-abcd--ferranti-etkisi-p1)
17. [RLC Geçici Rejim (Transient) Basamak Yanıtı (P2)](#17-rlc-geçici-rejim-transient-basamak-yanıtı-p2)
18. [Grafiksel Konvolüsyon & Fourier Harmonik Sentezi (P2)](#18-grafiksel-konvolüsyon--fourier-harmonik-sentezi-p2)

---

## 1. Ana Arayüz & Genel Bakış

Platform açıldığında sizi karşılayan ana çalışma istasyonu; modern **2026 Obsidian Gece Teması** ve **Pastel Gündüz Teması** seçenekleri, `Ctrl + K` hızlı arama çubuğu ve procedurally-generated (algoritmik çizilen) interaktif PCB arka planı ile donatılmıştır.

![Devrem Studio Ana Arayüz](images/overview/devrem_studio_hero.png)

* **Spotlight Arama (`Ctrl + K`):** Saniyeler içinde 27 laboratuvar aracına, sınav sorularına veya formüllere doğrudan odaklanmanızı sağlar.
* **Akıllı Yarıyıl & Track Filtresi:** 8 yarıyıl arasında geçiş ve Güç, RF, Kontrol, Gömülü Sistemler ve Çekirdek Mühendislik uzmanlaşma filtreleri.

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

---

## 10. KaTeX Matematiksel Formül Flashcard'ları

Sınavlara hazırlanan mühendislik öğrencileri için formül ezberleme ve soru-cevap kartları.

| Soru / Ön Yüz (Koyu) | Detaylı Çözüm / Arka Yüz (Koyu) |
| :---: | :---: |
| ![Flashcard Ön Koyu](images/flashcards/flashcard_on_yuz_koyu.png) | ![Flashcard Arka Koyu](images/flashcards/flashcard_arka_yuz_koyu.png) |

---

## 11. 8 Yarıyıl / 240 AKTS Bologna Müfredatı & Laboratuvar Köprüsü

Mühendislik eğitiminde teori ve pratik arasındaki kopukluğu gidermek amacıyla geliştirilen Bologna modülü;
- 8 yarıyılın tamamını (her biri 30 AKTS = toplam 240 AKTS) içerir.
- 4 uzmanlaşma alanı etiketine (`power`, `rf`, `control`, `embedded`, `core`) göre dinamik filtreleme sağlar.
- Canlı arama çubuğu ile ders kodu veya adına göre anında süzme yapar.
- Ders kartları üzerindeki `🚀 Laboratuvarda Aç: [Simülatör Adı]` butonu, ilgili laboratuvar modülünü doğrudan o derse özel ayarlarıyla başlatır.

---

## 12. Transformatör Eşdeğer Devre Simülatörü (P0)

![Transformatör Eşdeğer Devre Simülatörü](images/simulators/transformator_esdeger_koyu.png)


Elektrik makineleri laboratuvarlarında gerçekleştirilen standart **Boşta Çalışma (OC)** ve **Kısa Devre (SC)** deneylerini modeller:
* **Girdiler:** $V_{oc}, I_{oc}, P_{oc}$ ve $V_{sc}, I_{sc}, P_{sc}$, anma gücü $S_n$, dönüştürme oranı $a = N_1/N_2$, yükleme yüzdesi ve $\cos\phi$.
* **Çıktılar:** Nüve direnci $R_c$, mıknatıslanma reaktansı $X_m$, eşdeğer sargı direnci $R_{eq}$, kaçak reaktans $X_{eq}$, demir kayıpları $P_{fe}$, bakır kayıpları $P_{cu}$, tam verim $\eta$ ve gerilim regülasyonu $%VR$.
* **Fazör Kanvası:** $V_1$ primer gerilimi, $V_2'$ indirgenmiş sekonder gerilimi, $I_2'R_{eq}$ ohmik düşümü ve $jI_2'X_{eq}$ reaktif düşümünü gösteren dinamik fazör üçgeni.

---

## 13. 3-Faz Zikzak (Zn) & Vektör Saat Kadranı (P0)

Dağıtım şebekelerinde dengesiz tek fazlı yükleri dengelemek ve 3. harmonikleri nötrlemek için kullanılan zikzak sargı analizörü:
* **Desteklenen Gruplar:** Dyn11, Ynd1, Yzn5, Dzn0, Yy0.
* **Sargı Faktörü:** $k_w = \frac{\sqrt{3}}{2} \approx 0.866$ faktörü nedeniyle normal yıldız sargıya göre $%15.5$ daha fazla bakır sargı gereksinimi hesaplanır.
* **3. Harmonik Sıfırlama:** Her faza ait sargı iki farklı bacağa ters yönde sarıldığından $\Phi_{0,net} = 0$ olur ve nötr akımı dengelenir.
* **Kadran & Klemens:** 12 saat kadranında faz açı farkı ve $U-V-W / u-v-w$ klemens polarite bağlantı şeması.

---

## 14. Güç Elektroniği DC-DC Dönüştürücü & 3-Kanal Osiloskop (P1)

![DC-DC Dönüştürücü 3-Kanal Osiloskop](images/simulators/dcdc_donusturucu_koyu.png)


Anahtarlamalı güç kaynaklarının (SMPS) temel topolojilerini simüle eder:
* **Topolojiler:** Buck (Düşürücü), Boost (Yükseltici), Buck-Boost.
* **Kritik Endüktans:** $L_{crit} = \frac{(1-D)R}{2f_s}$ bağıntısıyla devrenin Sürekli İletim Modunda (CCM) mı yoksa Kesintili İletim Modunda (DCM) mı çalıştığı anlık tespit edilir.
* **3-Kanallı Osiloskop:**
  * Kanal 1 (Mavi): Bobin akımı $i_L(t)$ — üçgen yükselme/düşme ve DCM taban çizgisi.
  * Kanal 2 (Kırmızı): MOSFET anahtar gerilimi $v_{sw}(t)$ — iletimde $0V$, kesimde $V_{in}$ veya $V_{out}$.
  * Kanal 3 (Yeşil): Diyot akımı $i_D(t)$ — anahtar kesimdeyken yükü besleyen deşarj akımı.

---

## 15. Asenkron Motor Tork-Hız & V/f Sürücü Lab (P1)

![Asenkron Motor Kloss Tork Hız](images/simulators/asenkron_motor_koyu.png)


Endüstriyel sürücülerde kullanılan sincap kafesli asenkron motor tork-hız karakteristiği:
* **Thevenin & Kloss Modellemesi:** Motor eşdeğer devre parametrelerinden devrilme kayması $s_{max}$ ve devrilme torku $T_{max}$ türetilir; Kloss formülüyle tam $0 \le n \le n_s$ tork eğrisi oluşturulur.
* **Skaler $V/f$ Sürücü:** 15 Hz ile 75 Hz arasında frekans değiştirildiğinde gerilim/frekans oranı sabit tutularak tork eğrisi hız ekseninde kaydırılır; anma frekansının (50 Hz) üzerinde alan zayıflatma bölgesine geçilir.
* **HUD Göstergesi:** Kalkış torku $T_{st}$, anma torku $T_n$, devrilme torku $T_{max}$, senkron devir $n_s$ ve mekanik devir $n$.

---

## 16. Güç Sistemleri İletim Hattı, ABCD & Ferranti Etkisi (P1)

Yüksek gerilim enerji iletim hatlarında iki kapılı zincir parametreleri ve reaktif güç yönetimi:
* **Hat Modelleri:** Kısa ($<80$ km), Nominal $\pi$ (80–250 km) ve Nominal T hat modelleri.
* **Ferranti Olayı:** Yüksüz veya hafif yüklü uzun hatlarda kapasitif şarj akımının hat endüktansında oluşturduğu gerilim yükselmesi ($V_{R,0} = V_S / A > V_S$) hesaplanır.
* **Kompanzasyon:** İstenen güç faktörüne ulaşmak için şönt kondansatör bankı gücü $\Delta Q$ ve üçgen bağlı kapasite $C_\Delta$ hesaplanır.

---

## 17. RLC Geçici Rejim (Transient) Basamak Yanıtı (P2)

Darbe veya basamak gerilimi uygulanan Seri ve Paralel RLC devrelerinin analitik zaman düzlemi çözümleri:
* **Sönüm Rejimleri:**
  * $\zeta > 1$: Aşırı sönümlü (Overdamped, çift reel kök, salınımsız yavaş yükselme)
  * $\zeta = 1$: Kritik sönümlü (Critically damped, en hızlı aşımı olmayan oturma)
  * $0 < \zeta < 1$: Eksik sönümlü (Underdamped, sönümlü sinüsoidal salınım)
* **Kritik Metrikler:** Tepe aşımı $M_p = e^{-\pi\zeta / \sqrt{1-\zeta^2}}$, oturma zamanı $t_s \approx \frac{4}{\zeta\omega_0}$ ve sönümlü doğal frekans $\omega_d = \omega_0\sqrt{1-\zeta^2}$.

---

## 18. Grafiksel Konvolüsyon & Fourier Harmonik Sentezi (P2)

Doğrusal ve zamanla değişmeyen (LTI) sistemlerin çekirdek prensipleri:
* **Kayan İntegrasyon:** $y(t) = \int_{-\infty}^{\infty} x(\tau)h(t-\tau)d\tau$ integrasyonunu canlı animasyonla canlandırır. $x(t)$ sinyali sabit dururken $h(t)$ zaman tersi alınarak ($h(-\tau)$) soldan sağa kaydırılır ve kesişim alanı hesaplanır.
* **Etkileşim:** Başlat, Duraklat, Zamanı Sıfırla butonları ve serbest zaman ($t$) kaydırıcısı.
* **Fourier Serisi:** $N=1$ ile $N=49$ arasındaki tek harmoniklerin üst üste binmesiyle kare dalga üretimi ve $%8.95$ Gibbs olayı tepe sıçraması gösterimi.

---

*Devrem Studio - Elektrik-Elektronik Mühendisliği Profesyonel Çalışma İstasyonu*


## 19. Karnaugh Haritası (K-Map) Çözücü & Mantık Sentezi

![K-Map Çözücü ve Mantık Sentezi](images/simulators/kmap_cozucu_koyu.png)

* **Değişken Seçimi:** 2, 3 veya 4 değişkenli Gray kodlu Karnaugh haritası seçilir.
* **Hücre Değerleri:** Hücrelere tıklanarak 0, 1 ve Don't Care ($X$) durumları ayarlanır.
* **Otomatik Gruplama & Çözüm:** Quine-McCluskey algoritması en büyük $2^k$ boyutlu grupları bularak sadeleştirilmiş Çarpımlar Toplamı (SOP) fonksiyonunu üretir.

---

## 20. SMPS Buck / Boost Güç Elektroniği Tasarımcısı

![SMPS Buck Boost Tasarım Simülatörü](images/simulators/smps_tasarimci_koyu.png)

* **Topoloji:** Buck (Düşürücü) veya Boost (Yükseltici) seçimi yapılır.
* **Tasarım Kriterleri:** $V_{in}, V_o, I_o, f_s$ ve izin verilen dalgalanma oranları girilir.
* **Kritik Değerler:** $L_{min}, C_{min}$, akım tepe değeri ($I_{pk}$) ve CCM/DCM çalışma rejimi osiloskop ekranında canlı izlenir.

---

## 21. RF Mikroşerit Hat (Microstrip) Empedansı & 50Ω Sentezi

![RF Mikroşerit Hat Empedansı ve 50 Ohm Sentezi](images/simulators/rf_mikroserit_koyu.png)

* **Dielektrik Seçimi:** FR-4 ($\varepsilon_r=4.4$), Rogers RO4003C ($\varepsilon_r=3.55$) veya PTFE ($\varepsilon_r=2.1$) seçilir.
* **Parametreler:** Yükseklik ($H$), bakır kalınlığı ($T$) ve hat genişliği ($W$) girilir; Wheeler & Hammerstad formülleriyle $Z_0$ hesaplanır.
* **50Ω Otomatik Sentez:** "50Ω Sentezle" butonuna tıklandığında hedef empedansı veren hat genişliği mikron hassasiyetinde bulunur.

---

## 22. DC Motor & H-Bridge PWM Sürüş Simülasyonu

![DC Motor H-Bridge PWM Sürüş Simülatörü](images/simulators/dc_motor_koyu.png)

* **Çalışma Modları:** İleri, Geri, Fren ve Boşta modları arasında geçiş yapılır.
* **PWM Sürüşü:** PWM görev oranı kaydırılarak motor devri ($n$), armatür akımı ($I_a$) ve mekanik tork dinamik olarak izlenir.
* **Rejeneratif Frenleme:** Dış yük torku ve kinetik enerjinin kaynağa geri beslenmesi simüle edilir.

---

## 23. İnteraktif Eğri Takibi (Snapping), HUD Tooltip & Dokunsal Simülasyon
* **Eğriye Yapışma (Snapping):** Fare veya parmak kanvas üzerinde hareket ettirildikçe kılcal çizgiler ve hedef noktaları doğrudan en yakın fonksiyona yapışır.
* **Karanlık Cam HUD:** Anlık zaman, frekans, gerilim, akım, tork ve faz değerleri yüzen bilgi kartında okunur.
* **Dokunsal Geri Bildirim:** Simüle et butonuna tıklandığında mikro-titreşim ve yükleme animasyonuyla canlı dalga yayılımı devreye girer.
