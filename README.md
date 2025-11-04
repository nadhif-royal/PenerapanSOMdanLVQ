# Penerapan Jaringan Saraf Tiruan SOM dan LVQ untuk Pengenalan Pola pada Dataset Iris

Ini adalah proyek untuk mata kuliah Jaringan Saraf Tiruan (JST) di Fakultas Ilmu Komputer, Universitas Brawijaya. Proyek ini berfokus pada implementasi dua metode Jaringan Saraf Tiruan, yaitu **Self-Organizing Map (SOM)** dan **Learning Vector Quantization (LVQ)**, untuk melakukan pengenalan pola pada dataset Iris.

## 📖 Tentang Proyek

Tujuan utama dari proyek ini adalah untuk membandingkan kemampuan dua pendekatan JST:

1.  **Self-Organizing Map (SOM)**: Digunakan sebagai metode *unsupervised learning* (pembelajaran tanpa pengawasan). SOM bertujuan untuk mengelompokkan data berdasarkan kesamaan fitur dan memvisualisasikan struktur data dalam peta 2D (U-Matrix).
2.  **Learning Vector Quantization (LVQ)**: Digunakan sebagai metode *supervised learning* (pembelajaran dengan pengawasan). LVQ menggunakan prototipe untuk mewakili setiap kelas dan melatihnya untuk melakukan klasifikasi data.

Dataset yang digunakan adalah **Iris dataset**, yang berisi 150 sampel dari 3 spesies bunga (Setosa, Versicolor, dan Virginica).

## ⚙️ Alur Metodologi

Penelitian ini dilakukan dengan alur sebagai berikut:

1.  **Import Library & Load Dataset**: Memuat *library* yang diperlukan (seperti MiniSom dan Scikit-learn) dan memuat dataset Iris.
2.  **Preprocessing Data**: Melakukan standarisasi fitur menggunakan `StandardScaler` agar setiap fitur memiliki skala yang seimbang.
3.  **Training SOM & Visualisasi**: Melatih model SOM pada data yang telah distandarisasi dan memvisualisasikan hasilnya menggunakan **U-Matrix** untuk melihat batas-batas klaster.
4.  **Mapping Label**: Memetakan label asli data ke peta SOM untuk menganalisis sebaran klaster alami.
5.  **Training LVQ (Supervised)**: Membagi data menjadi 70% latih dan 30% uji, kemudian melatih model LVQ untuk melakukan klasifikasi.
6.  **Evaluasi**: Mengevaluasi kinerja model LVQ menggunakan metrik Akurasi, *Confusion Matrix*, dan *Classification Report*.

## 📊 Hasil

Hasil eksperimen menunjukkan bahwa kedua metode saling melengkapi:

* **SOM (Unsupervised)**: Visualisasi U-Matrix dan pemetaan label berhasil menunjukkan struktur data. Terlihat jelas bahwa *Iris Setosa* sangat berbeda dan terpisah dari dua kelas lainnya, sementara *Iris Versicolor* dan *Iris Virginica* memiliki karakteristik yang mirip dan tumpang tindih.
* **LVQ (Supervised)**: Model klasifikasi LVQ mampu membedakan ketiga kelas dengan baik. Pada evaluasi akhir, model berhasil mencapai akurasi **93.33%**.

## 🚀 Cara Menjalankan

Eksperimen ini dilakukan sepenuhnya di Google Colab.

1.  *Clone* repositori ini.
2.  Buka berkas `.ipynb` (LK4JST.ipynb) menggunakan Google Colaboratory.
3.  Alternatifnya, Anda dapat langsung membuka *notebook* melalui tautan berikut:
    * **[Buka di Google Colab](https://colab.research.google.com/drive/1N3dWDfZIgIwBwdvybZxxa94Nkn3BT0iX?usp=sharing)**
4.  Jalankan sel kode secara berurutan dari atas ke bawah.

## 🛠️ Teknologi dan Library

* Python 3.10
* Google Colab
* `minisom`
* `scikit-learn`
* `numpy`
* `pandas`
* `matplotlib`

## 👨‍💻 Tim Penyusun

* **Fikri Adyatma** (235150201111015)
* **Nadhif Rif’at Rasendriya** (235150201111074)
* **Afriza Herdian Adicandra** (235150201111013)

---
Program Studi Teknik Informatika
Fakultas Ilmu Komputer
Universitas Brawijaya 2025
