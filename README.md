# 🧠 TensorFlow & Keras ile Derin Öğrenme Uygulamaları

Bu depoda, **TensorFlow / Keras** kütüphaneleri kullanılarak geliştirilmiş farklı Derin Öğrenme (Deep Learning) problemleri, model optimize etme yöntemleri ve sınıflandırma/regresyon projeleri yer almaktadır.

---

## 📂 Depo İçeriği ve Proje Detayları

### 1. 🚲 Bisiklet Fiyat Tahmin Modeli (Regresyon)
* **Veri Seti:** `bisiklet_fiyatlari.xlsx`
* **Amaç:** Bisiklet özelliklerine göre fiyat tahmini yapılması.
* **Öne Çıkanlar:**
  * Verilerin `MinMaxScaler` ile 0-1 aralığına ölçeklenmesi.
  * `Sequential` mimari ile katmanlı Sinir Ağı oluşturulması.
  * Modelin eğitilip kaydedilmesi (`bisiklet_modeli.h5`) ve tekrar yüklenerek test verisi üzerinde tahmin çalıştırılması (`load_model`).

### 2. 🛡️ Malicious URL / Web Sitesi Tespiti (Binary Classification)
* **Veri Seti:** `maliciousornot.xlsx`
* **Amaç:** Bir web sitesinin güvenli mi yoksa zararlı mı (malicious) olduğunun sınıflandırılması.
* **Öne Çıkanlar:**
  * Sınıflandırma problemi için **Binary Crossentropy** kayıp fonksiyonu ve **Sigmoid** aktivasyonu kullanımı.
  * Korelasyon analizi ile hedef değişken üzerindeki etkilerin incelenmesi.

### 3. 🎯 Model Optimizasyonu: EarlyStopping & Dropout
* Overfitting (aşırı öğrenme) problemini önlemek için **EarlyStopping** callback'i ile eğitimin doğru anda durdurulması.
* Katmanlar arası bilgi ezberlemesini önlemek amacıyla **Dropout** katmanlarının modele entegre edilmesi.

---

## 🛠️ Kullanılan Teknolojiler

* **Python 3.x**
* **TensorFlow / Keras:** Model mimarisi, katmanlar (`Dense`, `Dropout`), callback'ler (`EarlyStopping`).
* **Pandas & NumPy:** Veri işleme ve matris operasyonları.
* **Matplotlib & Seaborn:** Kayıp (loss) ve doğruluk (accuracy) grafiklerinin çizdirilmesi.
* **Scikit-learn:** Data scaling ve train-test ayırımı.

---

## 🚀 Projeyi Yerelde Çalıştırma

1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/seymamrd/tensorflow-derin-ogrenme.git](https://github.com/seymamrd/tensorflow-derin-ogrenme.git)
   cd tensorflow-derin-ogrenme
