# ♻️ Waste Image Classification using Deep Learning (CNN, MobileNet, ResNet50)

Proyek *Machine Learning* untuk mengklasifikasikan jenis material limbah berdasarkan gambar menggunakan arsitektur **Convolutional Neural Network (CNN)**. Proyek ini membandingkan beberapa arsitektur *Deep Learning* (MobileNet, ResNet50, dan Custom CNN) untuk mendapatkan performa klasifikasi sampah dengan akurasi terbaik guna mendukung sistem pengelolaan limbah otomatis.

---

## 📌 Deskripsi Proyek

Sistem ini memproses masukan berupa gambar sampah dan mengategorikannya ke dalam salah satu dari 10 kelas spesifik. Dengan membandingkan model ringan (MobileNet) dan model dalam (ResNet50), proyek ini menganalisis keseimbangan antara ukuran model, kecepatan komputasi, dan tingkat akurasi klasifikasi. Seluruh alur mulai dari *preprocessing*, pelatihan (*training*), hingga pengujian model dilakukan di dalam *Jupyter Notebook*.

---

## 📊 Dataset & Kategori Sampah

Dataset yang dilatih terdiri dari 10 kelas direktori jenis limbah:
- 🔋 **Battery** (Baterai)
- 🍎 **Biological** (Sampah Organik/Biologis)
- 📦 **Cardboard** (Kardus)
- 👕 **Clothes** (Pakaian/Kain)
- 🍾 **Glass** (Kaca)
- 🥫 **Metal** (Logam/Kaleng)
- 📄 **Paper** (Kertas)
- 🛍️ **Plastic** (Plastik)
- 👟 **Shoes** (Sepatu)
- 🗑️ **Trash** (Sampah Campuran/Lainnya)

---

## 🧠 Arsitektur Model yang Dievaluasi

Terdapat tiga model terlatih (format `.h5`) yang dievaluasi dalam proyek ini:
1. **`mobilenet_sampah.h5`:** Menggunakan *pre-trained model* **MobileNet**. Model yang sangat ringan dan efisien, cocok diimplementasikan pada perangkat *Edge* atau ponsel cerdas.
2. **`resnet50_sampah.h5`:** Menggunakan *pre-trained model* **ResNet50**. Arsitektur yang lebih dalam dan unggul dalam mengenali pola gambar yang rumit dengan akurasi tinggi.
3. **`model_1_cnn_sampah.h5`:** Model arsitektur CNN dasar (Custom CNN) yang dirancang dari awal secara mandiri.

---

## 📁 Struktur Repositori

```text
├── dataset/                   # Dataset utama yang berisi 10 kelas gambar jenis sampah
├── sampahtes/                 # Folder berisi data gambar (*unseen data*) untuk pengetesan akhir
├── mobilenet_sampah.h5        # File model terlatih MobileNet (11 MB)
├── model_1_cnn_sampah.h5      # File model terlatih Custom CNN (130 MB)
├── resnet50_sampah.h5         # File model terlatih ResNet50 (211 MB)
├── sampah1.ipynb              # Jupyter Notebook berisi seluruh script AI (Training & Evaluation)
└── README.md                  # Dokumentasi proyek
