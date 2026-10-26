# 🌍 3D Dünya Yer Çekimi İvmesi ($g$) Simülasyonu

Bu proje, Fizik I dersi ödevi kapsamında geliştirilmiş; Dünya üzerindeki konum (enlem) ve yüksekliğe (rakım) bağlı olarak yer çekimi ivmesindeki ($g$) değişimi interaktif olarak hesaplayan ve 3 boyutlu olarak görselleştiren bir web simülasyonudur.

🚀 **Canlı Uygulama:** [ademkaleli.github.io/fizik1-yercekimi-odevi](https://ademkaleli.github.io/fizik1-yercekimi-odevi/)

---

## 👤 Öğrenci Bilgileri

* **Adı Soyadı:** Adem Kaleli
* **Öğrenci No:** 2615501083
* **Ders:** Fizik I
* **Ödev Konusu:** Dünya Üzerinde Konuma ve Rakıma Göre Yer Çekimi İvmesi ($g$) Değişimi Simülasyonu

---

## 🧮 Fiziksel Denklemler ve Matematiksel Model

Simülasyonda, Uluslararası Geodezi Formülü olan **Somigliana Denklemi** ve **Serbest Hava Yükseklik Düzeltmesi (Free-Air Correction)** kullanılmıştır:

$$g(\phi, h) = 9.780327 \times \left(1 + 0.0053024 \sin^2\phi - 0.0000058 \sin^2(2\phi)\right) - 3.086 \times 10^{-6} \times h$$

* $\phi$: Konumun enlemi (derece)
* $h$: Deniz seviyesinden yükseklik / rakım (metre)
* $g$: Hesaplanan yer çekimi ivmesi ($\text{m/s}^2$)

### Temel Fizik Mantığı
1. **Enlem Etkisi:** Dünya kutuplardan basık olduğu için kutuplar merkeze daha yakındır ve merkezkaç kuvveti sıfırdır. Bu nedenle enlem arttıkça yer çekimi artar ($\approx 9.832 \text{ m/s}^2$).
2. **Rakım Etkisi:** Deniz seviyesinden yukarı çıkıldıkça Dünya merkezinden uzaklaşıldığı için çekim kuvveti azalır (örneğin Everest Tepesi'nde $\approx 9.765 \text{ m/s}^2$).

---

## ✨ Özellikler

* 🌐 **İnteraktif 3D Küre:** Three.js (WebGL) kütüphanesi kullanılarak 3 boyutlu Dünya modeli ve atmosfer ışıması.
* 📱 **Tam Mobil ve Dokunmatik Desteği:** Masaüstü fare kontrolleri ve mobil cihazlarda dokunmatik yüzey hassasiyeti (Pointer Events).
* 📍 **Rastgele Konum Seçimi:** Dünya yüzeyinde herhangi bir noktaya dokunulduğunda koordinatların (Enlem & Boylam) anlık tespiti ve canlı $g$ hesabı.
* ⚡ **Hızlı Konum Butonları:** Ankara, İstanbul, Burdur, Antalya, Quito, Kuzey Kutbu, Everest Tepesi ve Ölü Deniz için tek tıkla odaklanma.
* 🎨 **Öğrenci Künye Rozeti:** Ekran üzerinde öğrenci bilgilerini taşıyan özel saydam katman.

---

## 🛠️ Kullanılan Teknolojiler

* **HTML5 / CSS3** (Responsive & Dark Mode Arayüz)
* **JavaScript (ES6+)**
* **Three.js (r128)** (WebGL 3D Render Engine)
* **OrbitControls.js** (3D Kamera Kontrolü)

---

## 💻 Yerel Çalıştırma

Herhangi bir derleyici veya sunucu kurulumu gerektirmez.

1. Depoyu klonlayın veya indirin:
   ```bash
   git clone [https://github.com/ademkaleli/fizik1-yercekimi-odevi.git](https://github.com/ademkaleli/fizik1-yercekimi-odevi.git)
