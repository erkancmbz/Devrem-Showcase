# ⚡ Devrem Studio (EEM Rehber) — Architectural Showcase & Portfolio

> **Elektrik-Elektronik Mühendisleri İçin Sıfır-Kurulum, Web Tabanlı Profesyonel Çalışma & Gelişim İstasyonu**  
> *Bu depo, Devrem Studio projesinin mimarisini, laboratuvar araçlarını, ekran görüntülerini ve öğretici dokümantasyonunu sergileyen resmi vitrin (showcase) reposudur.*

---

[![Showcase](https://img.shields.io/badge/Showcase-Official_Architecture_Portfolio-6366f1?style=for-the-badge&logo=github&logoColor=white)](https://github.com/erkancmbz/Devrem-Showcase)
[![Mobile Performance](https://img.shields.io/badge/Mobile-60_FPS_Zero--Overflow-10b981?style=for-the-badge&logo=googlechrome&logoColor=white)](docs/OGRETICI_REHBER.md)
[![Pure Vanilla Stack](https://img.shields.io/badge/Stack-HTML5_|_CSS3_|_Vanilla_JS-f59e0b?style=for-the-badge&logo=javascript&logoColor=white)](docs/OGRETICI_REHBER.md)
[![Math Engine](https://img.shields.io/badge/Formulas-KaTeX_LaTeX_Engine-0284c7?style=for-the-badge&logo=latex&logoColor=white)](https://katex.org)
[![Audio Simulation](https://img.shields.io/badge/Oscilloscope-Web_Audio_API-a855f7?style=for-the-badge)](docs/OGRETICI_REHBER.md)
[![License: Non-Commercial](https://img.shields.io/badge/License-Non--Commercial_|_Gayri_Ticari-dc2626?style=for-the-badge)](LICENSE)

---

<div align="center">
  <img src="docs/images/overview/devrem_studio_hero.png" alt="Devrem Studio Hero Arayüzü" width="920" style="border-radius: 12px; box-shadow: 0 16px 40px rgba(0,0,0,0.6);">
  <br><br>
  <p><strong>Devrem Studio:</strong> Obsidian & Pastel Çift Tema Desteği, Gerçek Zamanlı Kanvas Simülatörleri ve İnteraktif EEM Laboratuvarı</p>
  <p>
    <a href="docs/OGRETICI_REHBER.md"><strong>📖 ➔ Resimli Görsel Öğretici & Adım Adım Modül Kullanım Rehberi İçin Tıklayın</strong></a>
  </p>
</div>

---

## 📌 1. Projenin Vizyonu ve Çıkış Noktası

Elektrik-Elektronik Mühendisliği (EEM) teknik açıdan dünyanın en yoğun ve geniş mühendislik disiplinlerinden biridir. Bir EEM öğrencisinin veya genç bir mühendisin karşılaştığı en büyük sorun **araçların ve bilginin aşırı dağınık olmasıdır**:

1. **Ağır ve Lisanslı Simülatör Bağımlılığı:** Basit bir RC/RLC filtre frekans tepkisini, fazör açısını veya 2. derece kontrol sistemi basamak yanıtını görmek için gigabaytlarca boyutundaki lisanslı programları (MATLAB/Simulink, LTspice) beklemek gerekir.
2. **Teorik Bilginin Parçalanması:** Maxwell denklemleri, Fourier/Laplace dönüşümleri ve analog devre analiz formülleri dağınık PDF'lerde kaybolur.
3. **Sektör ve Kariyer Kopukluğu:** Savunma sanayii (ASELSAN, BAYKAR, TUSAŞ) teknik mülakat hazırlığı, TEKNOFEST/TÜBİTAK çağrıları ve güncel staj fırsatları tek bir çatı altında toplanmamıştır.

### 🎯 Çözüm: Devrem Studio
**Devrem Studio**, herhangi bir kurulum veya bağımlılık gerektirmeksizin (`npm install` bile yok!), sadece tarayıcıyı açarak **cep telefonunda, tablette veya bilgisayarda** çalışan, EEM öğrencisinin 1. sınıftan mezuniyetine (ve ilk işine) kadar ihtiyaç duyacağı tüm hesaplayıcıları, simülatörleri, formülleri ve kariyer araçlarını tek bir modern çatı altında toplamaktadır.

---

## 📸 2. İnteraktif Mühendislik Simülatörleri & Laboratuvar Vitrini

Platform bünyesinde geliştirilen tüm simülasyon ve analiz araçları **HiDPI Retina uyumlu 2D Canvas Motoru** üzerinde sıfırdan matematiksel algoritmalarla inşa edilmiştir.

### 🔬 Canlı Filtre Tasarımcısı & Bode Eğrisi
> Analog alçak geçiren, yüksek geçiren, bant geçiren ve bant durduran filtrelerin kesim frekansı ($f_c$), sönümleme ve faz eğrilerini canlı logaritmik frekans skalasında çizer.

<div align="center">
  <img src="docs/images/simulators/bode_filtre_koyu.png" alt="Bode Plot Simülatörü Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/bode_filtre_acik.png" alt="Bode Plot Simülatörü Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 🎛️ 2. Derece Kontrol Sistemleri & Basamak Yanıtı (Step Response)
> Sönüm oranı ($\zeta$) ve doğal frekans ($\omega_n$) ayarı ile dinamik oturma zamanı ($T_s \pm \%2$), tepe aşımı ($M_p$) ve yükselme süresini interaktif HUD ile anlık gösterir.

<div align="center">
  <img src="docs/images/simulators/kontrol_sistemi_koyu.png" alt="Kontrol Sistemi Basamak Yanıtı Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/kontrol_sistemi_acik.png" alt="Kontrol Sistemi Basamak Yanıtı Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 📐 Fazör Analizörü & AC Trigonometrik İzdüşüm
> Kutupsal (Polar) ve Kartezyen karmaşık sayı dönüşümleri, açı ve genlik vektörlerinin canlı trigonometrik izdüşümü.

<div align="center">
  <img src="docs/images/simulators/fazor_analizi_koyu.png" alt="Fazör Analizi Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/fazor_analizi_acik.png" alt="Fazör Analizi Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 📡 Smith Chart RF Empedans Eşleme Simülatörü
> Yüksek frekans ve mikrodalga iletim hatlarında yansıma katsayısı ($\Gamma$), VSWR ve karakteristik empedans ($Z_0$) eşleme çemberlerini 1:1 dairesel geometriyle çizer.

<div align="center">
  <img src="docs/images/simulators/smith_chart_koyu.png" alt="Smith Chart RF Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/smith_chart_acik.png" alt="Smith Chart RF Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### ⚡ 3-Fazlı Güç & Yük Denge Analizörü
> Yıldız ($Y$) ve Üçgen ($\Delta$) bağlantılarda faz gerilimleri, fazör açıları, dengesiz yük durumunda nötr akımı ve Falstad simülasyon entegrasyonu.

<div align="center">
  <img src="docs/images/simulators/uc_faz_guc_koyu.png" alt="3 Faz Güç Simülatörü Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/uc_faz_guc_acik.png" alt="3 Faz Güç Simülatörü Açık Tema" width="440" style="border-radius: 8px;">
</div>

---

### 🔊 Web Audio Canlı Sinyal Jeneratörü & Op-Amp Osiloskobu
> Tarayıcının yerel ses işlemcisini kullanarak 20 Hz – 20 kHz gerçek ses frekansları üretir ve 7 farklı op-amp topolojisinde doyum ($V_{sat}$) kırpılmasını canlı osiloskopta simüle eder.

<div align="center">
  <img src="docs/images/simulators/opamp_osiloskop_koyu.png" alt="Opamp Osiloskop Koyu Tema" width="440" style="border-radius: 8px;">
  <img src="docs/images/simulators/sinyal_jeneratoru_koyu.png" alt="Sinyal Jeneratörü Koyu Tema" width="440" style="border-radius: 8px;">
</div>

---

## 📟 3. İnteraktif Mikrodenetleyici Pinout Görüntüleyici

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

## 🧠 4. 3D Kavram Kartları (Flashcards) & KaTeX Formül Motoru

Kitap kalitesinde LaTeX formül render'ı sunan KaTeX motoru ve sınavlara hazırlık için 3D dönen kavram kartları:

<div align="center">
  <img src="docs/images/flashcards/flashcard_on_yuz_koyu.png" alt="Flashcard Ön Yüz" width="440" style="border-radius: 8px;">
  <img src="docs/images/flashcards/flashcard_arka_yuz_koyu.png" alt="Flashcard Arka Yüz" width="440" style="border-radius: 8px;">
</div>

---

## 🏗️ 5. Sistem Mimarisi & Mühendislik Yaklaşımı

Devrem Studio, ağır kütüphane bağımlılıklarını reddeden saf web mühendisliği (Vanilla Craftsmanship) felsefesiyle inşa edilmiştir:

```
┌────────────────────────────────────────────────────────────────────────┐
│                        DEVREM STUDIO MİMARİSİ                          │
├────────────────────────────────┬───────────────────────────────────────┤
│  Arayüz & Tasarım Sistemi      │  Obsidian 2026 Dark & Pastel Light    │
│                                │  CSS3 3D Transforms & Glassmorphism   │
├────────────────────────────────┼───────────────────────────────────────┤
│  Grafik & Simülasyon Motoru    │  Pure HTML5 Canvas 2D (Retina HiDPI)  │
│                                │  Dynamic Mathematical Plotters        │
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
- **Donanım Hızlandırma:** Dokunmatik ekranlarda gereksiz fare dinleyicileri pasifleştirilmiş, 45 adet ağır blur katmanı optimize edilerek mobil işlemci ve pil tüketimi minimize edilmiştir.
- **Tam Ekran Mobil Shell:** Laboratuvar pencereleri mobilde native bir akıllı telefon uygulaması (`100vw / 100vh`) gibi açılır.

---

## 📖 6. Detaylı Öğretici Rehber

Tüm modüllerin tek tek nasıl çalıştığını, formül arka planlarını ve simülatör kullanım senaryolarını adım adım incelemek için resimli rehberimizi ziyaret edin:

👉 **[docs/OGRETICI_REHBER.md Dosyasına Git](docs/OGRETICI_REHBER.md)**

---

## ⚖️ 7. Lisans & Fikri Mülkiyet (Telif Bildirimi)

Bu depo ve Devrem Studio projesi, **PolyForm Noncommercial 1.0.0** ve **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** lisansları altında korunmaktadır:

- ✅ **Eğitim, inceleme ve kişisel gelişim amaçlı kullanım tamamen serbesttir.**
- ❌ **Ticari amaçla satış, gelir elde etme, kapalı kodlu ticari platformlara aktarma veya kurumsal lisanslama KESİNLİKLE YASAKTIR.**

Ayrıntılı yasal şartlar için [LICENSE](LICENSE) belgesini inceleyebilirsiniz.

---

<div align="center">
  <p><strong>Geliştirici & Tasarımcı:</strong> <a href="https://github.com/erkancmbz">Erkan Cambaz (@erkancmbz)</a></p>
  <p><em>"Mühendisler için, mühendislik tutkusuyla tasarlandı."</em></p>
</div>
