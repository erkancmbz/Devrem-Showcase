# ⚡ Devrem Studio (EEM Rehber) — Architectural Showcase & Portfolio

> **Elektrik-Elektronik Mühendisleri İçin Sıfır-Kurulum, Web Tabanlı Profesyonel Çalışma & Gelişim İstasyonu**  
> *Bu depo, Devrem Studio projesinin mimarisini, laboratuvar araçlarını, ekran görüntülerini ve öğretici dokümantasyonunu sergileyen resmi vitrin (showcase) reposudur.*

---

[![Showcase](https://img.shields.io/badge/Showcase-Official_Architecture_Portfolio-6366f1?style=for-the-badge&logo=github&logoColor=white)](https://github.com/erkancmbz/Devrem-Showcase)
[![Engineering Tools](https://img.shields.io/badge/Laboratory-23_Engineering_Tools-38bdf8?style=for-the-badge&logo=codepen&logoColor=white)](docs/OGRETICI_REHBER.md)
[![Bologna Curriculum](https://img.shields.io/badge/Curriculum-8_Semesters_|_240_AKTS-10b981?style=for-the-badge&logo=gitbook&logoColor=white)](docs/OGRETICI_REHBER.md)
[![Mobile Performance](https://img.shields.io/badge/Mobile-60_FPS_Zero--Overflow-10b981?style=for-the-badge&logo=googlechrome&logoColor=white)](docs/OGRETICI_REHBER.md)
[![Pure Vanilla Stack](https://img.shields.io/badge/Stack-HTML5_|_CSS3_|_Vanilla_JS-f59e0b?style=for-the-badge&logo=javascript&logoColor=white)](docs/OGRETICI_REHBER.md)
[![Math Engine](https://img.shields.io/badge/Formulas-KaTeX_LaTeX_Engine-0284c7?style=for-the-badge&logo=latex&logoColor=white)](https://katex.org)
[![Audio Simulation](https://img.shields.io/badge/Oscilloscope-Web_Audio_API-a855f7?style=for-the-badge)](docs/OGRETICI_REHBER.md)
[![License: Non-Commercial](https://img.shields.io/badge/License-Non--Commercial_|_Gayri_Ticari-dc2626?style=for-the-badge)](LICENSE)

---

<div align="center">
  <img src="docs/images/overview/devrem_studio_hero.png" alt="Devrem Studio Hero Arayüzü" width="920" style="border-radius: 12px; box-shadow: 0 16px 40px rgba(0,0,0,0.6);">
  <br><br>
  <p><strong>Devrem Studio:</strong> 8 Yarıyıl / 240 AKTS Bologna Lisans Müfredatı, 23 İnteraktif Mühendislik Aracı ve Donanım Hızlandırmalı Kanvas Simülatörleri</p>
  <p>
    <a href="docs/OGRETICI_REHBER.md"><strong>📖 ➔ Resimli Görsel Öğretici & Adım Adım Modül Kullanım Rehberi İçin Tıklayın</strong></a>
  </p>
</div>

---

## 📌 1. Projenin Vizyonu ve Çıkış Noktası

Elektrik-Elektronik Mühendisliği (EEM) teknik açıdan dünyanın en yoğun ve geniş mühendislik disiplinlerinden biridir. Bir EEM öğrencisinin veya genç bir mühendisin karşılaştığı en büyük sorun **araçların ve bilginin aşırı dağınık olmasıdır**:

1. **Ağır ve Lisanslı Simülatör Bağımlılığı:** Basit bir RC/RLC filtre frekans tepkisini, fazör açısını, transformatör eşdeğer devresini veya motor tork-hız karakteristiğini görmek için gigabaytlarca boyutundaki lisanslı programları (MATLAB/Simulink, LTspice, AutoCAD Electrical) beklemek gerekir.
2. **Müfredat ile Laboratuvar Kopukluğu:** Bologna 8 yarıyıllık lisans dersleri ile hesaplama araçları arasında doğrudan bir köprü bulunmaz; öğrenci formülleri izole PDF'lerden ezberler.
3. **Sektör ve Kariyer Kopukluğu:** Savunma sanayii (ASELSAN, BAYKAR, TUSAŞ) teknik mülakat hazırlığı, TEKNOFEST/TÜBİTAK çağrıları ve güncel staj fırsatları tek bir çatı altında toplanmamıştır.

### 🎯 Çözüm: Devrem Studio
**Devrem Studio**, herhangi bir kurulum veya bağımlılık gerektirmeksizin (`npm install` bile yok!), sadece tarayıcıyı açarak **cep telefonunda, tablette veya bilgisayarda** çalışan, EEM öğrencisinin 1. sınıftan mezuniyetine (ve ilk işine) kadar ihtiyaç duyacağı tüm hesaplayıcıları, simülatörleri, formülleri ve kariyer araçlarını tek bir modern çatı altında toplamaktadır.

---

## 🎓 2. 8 Yarıyıl / 240 AKTS Bologna Lisans Müfredatı & Akıllı Köprü

Devrem Studio, Türkiye ve dünyadaki mühendislik akreditasyon standartlarına (MÜDEK & ABET) uygun olarak hazırlanan **tam 8 yarıyıl / 240 AKTS lisans müfredatını** barındırır. Her dönem 30 AKTS'ye dengelenmiş 5 temel/seçmeli dersten oluşur:

| Yarıyıl | Odak Alanı & Temel Kazanımlar | AKTS | Örnek Dersler & Doğrudan Laboratuvar Köprüsü |
| :---: | :--- | :---: | :--- |
| **1. Yarıyıl (Güz)** | Mühendislik Temelleri & Kalkülüs | 30 | Fizik I, Kalkülüs I, EEM Giriş, Programlama ➔ *Temel Bilim Modülü* |
| **2. Yarıyıl (Bahar)** | DC Devre Analizi & Elektromanyetizma | 30 | Devre Analizi I, Kalkülüs II, Fizik II ➔ *DC Devre Çözücü & Direnç Ağları* |
| **3. Yarıyıl (Güz)** | AC Devre Analizi & Lojik Tasarım | 30 | Devre Analizi II, Lojik Devreler, Dif. Denklemler ➔ *Fazör Analizörü & Mantık Kapıları* |
| **4. Yarıyıl (Bahar)** | Yarıiletken Elektronik & Sinyaller | 30 | Elektronik I, Sinyaller & Sistemler, Alan Teorisi ➔ *Konvolüsyon & Fourier Sentezi* |
| **5. Yarıyıl (Güz)** | Op-Amp, RF & Gömülü Sistemler | 30 | Elektronik II, Mikroişlemciler, EM Dalgalar ➔ *Bode Filtre, MCU Pinout, Smith Chart* |
| **6. Yarıyıl (Bahar)** | Kontrol Sistemleri & Elektrik Makineleri | 30 | Otomatik Kontrol, Elektrik Makineleri, Güç İletimi ➔ *Transformatör, Motor, Zikzak Zn, ABCD* |
| **7. Yarıyıl (Güz)** | Güç Elektroniği & Sinyal İşleme | 30 | Güç Elektroniği, DSP, Bitirme Tasarımı I ➔ *DC-DC Dönüştürücü & 3-Kanal Osiloskop* |
| **8. Yarıyıl (Bahar)** | Bitirme Projesi, Etik & Sanayi | 30 | Bitirme Tasarımı II, Mühendislik Etiği, İleri Seçmeliler ➔ *Kariyer & Mülakat Simülasyonu* |

### 🚀 `Laboratuvarda Aç` Deep-Link Mimarisi
Tüm ders kartlarının üzerinde bulunan hızlı başlatma butonu, kullanıcının o derste işlenen teorik konunun laboratuvar simülatörüne tek tıkla doğrudan odaklanmasını sağlar (örn. *Elektrik Makineleri* kartından doğrudan *Transformatör Eşdeğer Devre Simülatörü*ne geçiş).

---

## 🔬 3. İnteraktif Mühendislik Simülatörleri (23 Araçlık Laboratuvar)

Platform bünyesinde geliştirilen tüm simülasyon ve analiz araçları **HiDPI Retina uyumlu 2D Canvas Motoru** üzerinde sıfırdan matematiksel algoritmalarla inşa edilmiştir.

### ⚡ 3.1 Transformatör Eşdeğer Devre & Boşta/Kısa Devre Testi (P0)
Boşta çalışma ($V_{oc}, I_{oc}, P_{oc}$) ve kısa devre ($V_{sc}, I_{sc}, P_{sc}$) deney verilerini işleyerek demir nüve ve sargı empedanslarını hesaplar:
$$R_c = \frac{V_{oc}^2}{P_{oc}}, \quad X_m = \frac{V_{oc}}{I_m}, \quad R_{eq} = \frac{P_{sc}}{I_{sc}^2}, \quad X_{eq} = \sqrt{Z_{eq}^2 - R_{eq}^2}$$
* **Yetkinlikler:** $%0 - %150$ yükleme oranı ve değişken $\cos\phi$ (ileri/geri) altında tam verim ($\eta$) ve gerilim regülasyonu ($\%VR$) hesaplar; $V_1, V_2', I_2'R_{eq}, jI_2'X_{eq}$ dinamik Canvas fazör diyagramını çizer.

---

### 🧭 3.2 3-Faz Zikzak (Zn) & Vektör Saat Kadranı Analizörü (P0)
Trafosuz nötr elde etme ve 3. harmonik yok etme amacıyla kullanılan zikzak sargı geometrisini modeller:
$$V_{zn} = \sqrt{3} \cdot V_{sargı} \cdot \cos(30^\circ), \quad k_w = \frac{\sqrt{3}}{2} \approx 0.866$$
* **Desteklenen Gruplar:** Dyn11, Ynd1, Yzn5, Dzn0, Yy0 vektör grupları.
* **Mühendislik Çıkarımı:** $\%15.5$ ilave bakır ihtiyacı, sıfır-bileşen akı nötrlenmesi ($\Phi_{0,net} = 0$) ve klemens bağlantı tablosu.

---

### 🔋 3.3 Güç Elektroniği DC-DC Dönüştürücü & 3-Kanal Osiloskop (P1)
Buck (Düşürücü), Boost (Yükseltici) ve Buck-Boost topolojilerinde süreksiz iletim modunu (DCM) ve kritik endüktansı hesaplar:
$$L_{crit} = \frac{(1-D)R}{2f_s}, \quad \Delta V_o = \frac{(1-D)V_o}{8LC f_s^2}$$
* **3-Kanal Osiloskop:** Bobin akımı $i_L(t)$, anahtar gerilimi $v_{sw}(t)$ ve diyot akımı $i_D(t)$ eşzamanlı dalga formları.

---

### ⚙️ 3.4 Asenkron Motor Tork-Hız & V/f Sürücü Lab (P1)
3-Fazlı sincap kafesli asenkron motorun Thevenin eşdeğeri ve Kloss bağıntısı üzerinden hız-tork eğrisini çizer:
$$T = \frac{2 T_{max}}{\frac{s}{s_{max}} + \frac{s_{max}}{s}}, \quad n_s = \frac{120 f}{P}$$
* **Skaler V/f Kontrolü:** 15 Hz – 75 Hz frekans kaydırıcısı ile sabit tork ve alan zayıflatma (Field Weakening) bölgelerini simüle eder; $T_{st}, T_n, T_{max}$ kritik noktalarını işaretler.

---

### 🗼 3.5 Güç Sistemleri İletim Hattı, ABCD & Ferranti Etkisi (P1)
Kısa, Nominal $\pi$ ve Nominal T modelleri üzerinde iki kapılı ABCD zincir matrisi analizi:
$$\begin{bmatrix} V_S \\ I_S \end{bmatrix} = \begin{bmatrix} A & B \\ C & D \end{bmatrix} \begin{bmatrix} V_R \\ I_R \end{bmatrix}, \quad V_{R,0} = \frac{V_S}{A}$$
* **Ferranti Etkisi:** Hafif yüklü ve yüksüz hatlarda alıcı uç gerilim yükselmesini ($V_{R,0} > V_S$) gösterir.
* **Kompanzasyon:** Hedef güç faktörü için reaktif güç ($\Delta Q$) ve üçgen kondansatör ($C_\Delta$) kapasite hesabı.

---

### ⏱️ 3.6 RLC Geçici Rejim (Transient) Basamak Yanıtı (P2)
Seri ve Paralel RLC devrelerinin 2. derece diferansiyel basamak yanıtını ($v_C(t), i_L(t)$) analitik olarak çözer:
$$\alpha = \frac{R}{2L}, \quad \omega_0 = \frac{1}{\sqrt{LC}}, \quad \zeta = \frac{\alpha}{\omega_0}$$
* Aşırı sönümlü ($\zeta > 1$), kritik sönümlü ($\zeta = 1$) ve eksik sönümlü ($0 < \zeta < 1$) rejim geçişleri.
* Dinamik tepe aşımı ($M_p$) ve yerleşme zamanı ($t_s \pm \%2$) HUD göstergeleri.

---

### 🌊 3.7 Grafiksel Konvolüsyon & Fourier Harmonik Sentezi (P2)
LTI sistemlerde sinyallerin zaman uzayında kayarak örtüşmesini ve alan integrasyonunu animasyonla sunar:
$$y(t) = \int_{-\infty}^{\infty} x(\tau)h(t-\tau)d\tau, \quad x_N(t) = \frac{4}{\pi} \sum_{k=1}^N \frac{\sin((2k-1)\omega_0 t)}{2k-1}$$
* Oynat, duraklat, zaman kaydırma ve sıfırlama kontrolleri.
* $N=1$ ile $N=49$ tek harmonik toplamıyla kare dalga sentezi ve $%8.95$ Gibbs aşımı gösterimi.

---

### 🔬 3.8 Canlı Filtre Tasarımcısı & Bode Eğrisi
> Analog alçak geçiren, yüksek geçiren, bant geçiren ve bant durduran filtrelerin kesim frekansı ($f_c$), sönümleme ve faz eğrilerini canlı logaritmik frekans skalasında çizer.

<div align="center">
  <img src="docs/images/simulators/bode_filtre_koyu.png" alt="Bode Plot Simülatörü Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/bode_filtre_acik.png" alt="Bode Plot Simülatörü Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 🎛️ 3.9 2. Derece Kontrol Sistemleri & Basamak Yanıtı
> Sönüm oranı ($zeta$) ve doğal frekans ($omega_n$) ayarı ile dinamik oturma zamanı ($T_s pm %2$), tepe aşımı ($M_p$) ve yükselme süresini interaktif HUD ile anlık gösterir.

<div align="center">
  <img src="docs/images/simulators/kontrol_sistemi_koyu.png" alt="Kontrol Sistemi Basamak Yanıtı Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/kontrol_sistemi_acik.png" alt="Kontrol Sistemi Basamak Yanıtı Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 📐 3.10 Fazör Analizörü & AC Trigonometrik İzdüşüm
> Kutupsal (Polar) ve Kartezyen karmaşık sayı dönüşümleri, açı ve genlik vektörlerinin canlı trigonometrik izdüşümü.

<div align="center">
  <img src="docs/images/simulators/fazor_analizi_koyu.png" alt="Fazör Analizi Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/fazor_analizi_acik.png" alt="Fazör Analizi Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 📡 3.11 Smith Chart RF Empedans Eşleme Simülatörü
> Yüksek frekans ve mikrodalga iletim hatlarında yansıma katsayısı ($Gamma$), VSWR ve karakteristik empedans ($Z_0$) eşleme çemberlerini 1:1 dairesel geometriyle çizer.

<div align="center">
  <img src="docs/images/simulators/smith_chart_koyu.png" alt="Smith Chart RF Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/smith_chart_acik.png" alt="Smith Chart RF Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### ⚡ 3.12 3-Fazlı Güç & Yük Denge Analizörü
> Yıldız ($Y$) ve Üçgen ($Delta$) bağlantılarda faz gerilimleri, fazör açıları, dengesiz yük durumunda nötr akımı ve Falstad simülasyon entegrasyonu.

<div align="center">
  <img src="docs/images/simulators/uc_faz_guc_koyu.png" alt="3 Faz Güç Simülatörü Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/uc_faz_guc_acik.png" alt="3 Faz Güç Simülatörü Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 🔊 3.13 Web Audio Canlı Sinyal Jeneratörü & Op-Amp Osiloskobu
> Tarayıcının yerel ses işlemcisini kullanarak 20 Hz – 20 kHz gerçek ses frekansları üretir ve 7 farklı op-amp topolojisinde doyum ($V_{sat}$) kırpılmasını canlı osiloskopta simüle eder.

<div align="center">
  <img src="docs/images/simulators/opamp_osiloskop_koyu.png" alt="Opamp Osiloskop Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/sinyal_jeneratoru_koyu.png" alt="Sinyal Jeneratörü Koyu Tema" width="440" style="border-radius: 8px;">
</div>

---

## 📟 4. İnteraktif Mikrodenetleyici Pinout Görüntüleyici

Gömülü sistem geliştiricileri için canlı SVG tabanlı mikrodenetleyici pinout şemaları:
- **Desteklenen Kartlar:** STM32F401 (BlackPill), ESP32 DevKit v1, Raspberry Pi Pico (RP2040), Arduino Uno R3.
- **Yetenekler:** I2C, SPI, UART, PWM, ADC ve Güç pinlerini dinamik butonlarla filtreleme; pin üzerine gelindiğinde anlık fonksiyon ve alternatif pin HUD paneli; dokunmatik mobilde pan-zoom kaydırma.

<div align="center">
  <img src="docs/images/pinouts/esp32_devkit_koyu.png" alt="ESP32 DevKit Pinout" width="440" style="border-radius: 8px;">
  <img src="docs/images/pinouts/stm32_blackpill_koyu.png" alt="STM32 BlackPill Pinout" width="440" style="border-radius: 8px;">
  <br><br>
  <img src="docs/images/pinouts/raspberry_pi_pico_koyu.png" alt="Raspberry Pi Pico Pinout" width="440" style="border-radius: 8px;">
  <img src="docs/images/pinouts/arduino_uno_koyu.png" alt="Arduino Uno Pinout" width="440" style="border-radius: 8px;">
</div>

---

## 🧠 5. 3D Kavram Kartları (Flashcards) & KaTeX Formül Motoru

Kitap kalitesinde LaTeX formül render'ı sunan KaTeX motoru ve sınavlara hazırlık için 3D dönen kavram kartları:

<div align="center">
  <img src="docs/images/flashcards/flashcard_on_yuz_koyu.png" alt="Flashcard Ön Yüz" width="440" style="border-radius: 8px;">
  <img src="docs/images/flashcards/flashcard_arka_yuz_koyu.png" alt="Flashcard Arka Yüz" width="440" style="border-radius: 8px;">
</div>

---

## 🏗️ 6. Sistem Mimarisi & Mühendislik Yaklaşımı

Devrem Studio, ağır kütüphane bağımlılıklarını reddeden saf web mühendisliği (Vanilla Craftsmanship) felsefesiyle inşa edilmiştir:

```
┌────────────────────────────────────────────────────────────────────────┐
│                        DEVREM STUDIO MİMARİSİ                          │
├────────────────────────────────┬───────────────────────────────────────┤
│  Arayüz & Tasarım Sistemi      │  Obsidian 2026 Dark & Pastel Light    │
│                                │  CSS3 3D Transforms & Glassmorphism   │
├────────────────────────────────┼───────────────────────────────────────┤
│  Grafik & Simülasyon Motoru    │  Pure HTML5 Canvas 2D (Retina HiDPI)  │
│  (23 Mühendislik Aracı)        │  Mathematical Real-Time Plotters      │
├────────────────────────────────┼───────────────────────────────────────┤
│  Müfredat & Akademik Motor     │  8 Yarıyıl / 240 AKTS Bologna Modeli  │
│                                │  4 Uzmanlaşma Pisti & Deep-Link Köprü │
├────────────────────────────────┼───────────────────────────────────────┤
│  Mobil Performans Motoru       │  IntersectionObserver API (0-Reflow)  │
│                                │  requestAnimationFrame 60 FPS Throttle│
├────────────────────────────────┼───────────────────────────────────────┤
│  Ses & Frekans Simülasyonu     │  Web Audio API (Hardware Synthesis)   │
├────────────────────────────────┼───────────────────────────────────────┤
│  Matematik & LaTeX Motoru      │  KaTeX High-Performance Math Engine   │
├────────────────────────────────┼───────────────────────────────────────┤
│  Veri & Durum Yönetimi         │  Offline-First LocalStorage System    │
└────────────────────────────────┴───────────────────────────────────────┘
```

### 📱 Mobil & Performans Garantisi
- **Sıfır Yatay Taşma (0 Horizontal Overflow):** 360px, 375px, 390px, 412px, 430px ekranlarda `scrollWidth === innerWidth` garantisi.
- **Donanım Hızlandırma:** Dokunmatik ekranlarda gereksiz fare dinleyicileri pasifleştirilmiş, ağır blur katmanları optimize edilerek mobil işlemci ve pil tüketimi minimize edilmiştir.
- **Tam Ekran Mobil Shell:** Laboratuvar pencereleri mobilde native bir akıllı telefon uygulaması (`100vw / 100vh`) gibi açılır.

---

## 📖 7. Detaylı Öğretici Rehber

Tüm modüllerin tek tek nasıl çalıştığını, formül arka planlarını ve simülatör kullanım senaryolarını adım adım incelemek için resimli rehberimizi ziyaret edin:

👉 **[docs/OGRETICI_REHBER.md Dosyasına Git](docs/OGRETICI_REHBER.md)**

---

## ⚖️ 8. Lisans & Fikri Mülkiyet (Telif Bildirimi)

Bu depo ve Devrem Studio projesi, **PolyForm Noncommercial 1.0.0** ve **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** lisansları altında korunmaktadır:

- ✅ **Eğitim, inceleme ve kişisel gelişim amaçlı kullanım tamamen serbesttir.**
- ❌ **Ticari amaçla satış, gelir elde etme, kapalı kodlu ticari platformlara aktarma veya kurumsal lisanslama KESİNLİKLE YASAKTIR.**

Ayrıntılı yasal şartlar için [LICENSE](LICENSE) belgesini inceleyebilirsiniz.

---

<div align="center">
  <p><strong>Geliştirici & Tasarımcı:</strong> <a href="https://github.com/erkancmbz">Erkan Cambaz (@erkancmbz)</a></p>
  <p><em>"Mühendisler için, mühendislik tutkusuyla tasarlandı."</em></p>
</div>
