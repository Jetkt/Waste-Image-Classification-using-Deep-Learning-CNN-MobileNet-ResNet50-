# ♻️ Waste Classification using Deep Learning (CNN, MobileNet, ResNet50)

Repositori ini berisi file **Jupyter Notebook (`sampah1.ipynb`)** yang memuat seluruh alur eksperimen *Deep Learning* untuk klasifikasi citra sampah ke dalam **10 kategori**. 

Di dalam notebook ini, telah dijalankan pelatihan dan evaluasi komprehensif yang membandingkan tiga arsitektur model: **Custom CNN**, **MobileNet**, dan **ResNet50**.

---

## 📌 Ringkasan Eksperimen

- **Tujuan:** Mengklasifikasikan gambar sampah secara otomatis berdasarkan jenis materialnya guna mendukung sistem pemilahan limbah otomatis.
- **Kategori Sampah (10 Kelas):** 
  - `battery` (baterai)
  - `biological` (organik/biologis)
  - `cardboard` (kardus)
  - `clothes` (pakaian/kain)
  - `glass` (kaca)
  - `metal` (logam)
  - `paper` (kertas)
  - `plastic` (plastik)
  - `shoes` (sepatu)
  - `trash` (sampah umum/campuran)
- **Model yang Dibandingkan:**
  1. **Custom CNN** (Model CNN kustom yang dibangun dari awal)
  2. **MobileNet** (*Transfer Learning* - Arsitektur ringan & cepat)
  3. **ResNet50** (*Transfer Learning* - Arsitektur *Deep Residual Network*)

---

## 📊 Hasil Evaluasi & Metrik Performa

Seluruh keluaran (*output*) pada notebook `sampah1.ipynb` telah tersimpan dan dapat dilihat langsung tanpa perlu menjalankan ulang (*re-run*) kode.

Metrik evaluasi yang disajikan di dalam notebook mencakup:
- **Confusion Matrix:** Melihat tingkat ketepatan dan kesalahan klasifikasi antar-kelas sampah.
- **Precision, Recall, & F1-Score:** Metrik evaluasi detail untuk setiap kelas (10 jenis sampah).
- **Kurva Evaluasi (F1-Curve / Accuracy & Loss Curve):** Visualisasi performa model selama proses *training* dan *validation*.
- **Hasil Pengujian (Inference Test):** Sampel gambar dari folder pengetesan beserta hasil prediksi dari model.

---

## 📁 Struktur Repositori

```text
├── sampah1.ipynb    # Jupyter Notebook utama (Pre-processing, Training, Evaluasi Metrik, & Pengetesan Model)
└── README.md        # Dokumentasi repositori
