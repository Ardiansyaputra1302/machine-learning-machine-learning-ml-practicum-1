<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

# 🏆 UTS: Mini Project End-to-End Machine Learning
### *Customer Personality Analysis (Customer Segmentation)*

**Praktikum Applied Machine Learning**  
**Program Studi Informatika - Universitas Muhammadiyah Makassar**

---
</div>

## 📌 Deskripsi Proyek
Proyek ini adalah tugas Ujian Tengah Semester (UTS) yang berfokus pada implementasi **Unsupervised Learning** secara *end-to-end*. Tujuan utama proyek ini adalah melakukan segmentasi pelanggan berdasarkan data demografi dan riwayat pengeluaran mereka untuk mengoptimalkan strategi *marketing campaign*.

## 📁 Tentang Dataset & Alasan Pemilihan
* **Nama Dataset**: Customer Personality Analysis
* **Sumber/Link Asli**: [Kaggle - Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
* **File Lokal**: `marketing_campaign.csv`

**Mengapa memilih dataset ini untuk UTS?**
1. **Relevansi Bisnis Dunia Nyata**: Dataset ini mensimulasikan tantangan nyata yang dihadapi tim pemasaran, di mana segmentasi yang buruk menyebabkan pemborosan anggaran iklan. Fokus penyelesaiannya langsung berdampak pada peningkatan *Return on Investment* (ROI).
2. **Karakteristik Data yang Kaya (*Rich Features*)**: Memiliki 29 kolom yang mencakup spektrum luas mulai dari demografi, struktur keluarga, hingga daya beli spesifik (daging, anggur, buah, dll), sehingga sangat menantang dan ideal untuk proses *Feature Engineering*.
3. **Kesesuaian dengan Unsupervised Learning**: Dataset ini tidak memiliki label klasifikasi segmentasi yang baku (tidak ada *target variable*). Hal ini menjadikannya kasus yang sempurna untuk diselesaikan menggunakan algoritma *Clustering* guna menemukan pola atau kelompok pelanggan yang tersembunyi secara otomatis.

## 🎯 Capaian Pembelajaran (Objectives)
- Melakukan **Exploratory Data Analysis (EDA)** untuk memahami distribusi demografi dan korelasi pengeluaran pelanggan.
- Melakukan **Data Preprocessing & Feature Engineering** (menangani *missing values*, *outliers*, dan *Standard Scaling*).
- Melatih dan membandingkan algoritma **K-Means** dan **Hierarchical Clustering (Agglomerative)**.
- Mengevaluasi model menggunakan metrik **Silhouette Score** dan **Elbow Method**.
- Menyusun **Business Recommendation** yang dapat ditindaklanjuti untuk setiap klaster.

## 🛠️ Tech Stack & Metode
* **Bahasa Pemrograman:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
* **Algoritma Machine Learning:**
  * K-Means Clustering
  * Hierarchical Clustering (Ward Linkage)
* **Evaluasi:** Silhouette Score

## 📊 Ringkasan Hasil Evaluasi
Dalam proyek ini, jumlah klaster optimal yang dipilih adalah **K=4**. Berikut adalah perbandingan performa model yang dievaluasi menggunakan *Silhouette Score*:

| Model | Silhouette Score | Keterangan |
|-------|------------------|------------|
| **K-Means** | `0.3270` | **Model Terbaik** (Pemisahan lebih baik) |
| **Hierarchical** | `0.2868` | Memiliki tingkat *overlap* yang lebih tinggi |

## 💡 Kesimpulan Segmen Pelanggan (Business Profiling)
Berdasarkan hasil K-Means (K=4), pelanggan berhasil dikelompokkan ke dalam 4 persona utama:

1. 🌟 **The Stars (High Income, High Spender):** Pelanggan VIP tanpa tanggungan anak yang membeli produk premium. Strategi: *Customer Retention* dan penawaran eksklusif.
2. 🚀 **The Potentials (Medium-High Income, Medium Spender):** Keluarga kecil dengan daya beli kuat. Strategi: Promosi *cross-selling* dan paket *bundling* keluarga.
3. 👨‍👩‍👧‍👦 **The Thrifty Parents (Medium Income, Low Spender):** Keluarga dengan banyak anak yang sensitif terhadap harga. Strategi: Diskon reguler, promo bahan pokok, dan kampanye ramah anggaran.
4. 📉 **The Minimalists (Low Income, Lowest Spender):** Pelanggan muda/lajang dengan pengeluaran minim. Strategi: Kampanye *entry-level*, *flash-sale*, dan adopsi aplikasi gratis.

## 📁 Struktur File
* `main.ipynb`: *Source code* utama (Jupyter Notebook) yang berisi seluruh tahapan dari Part 1 hingga Part 6.
* `marketing_campaign.csv`: Dataset mentah yang digunakan untuk analisis.
* `*.pdf`: Laporan hasil eksekusi *notebook* yang disubmit untuk penilaian UTS.

---
**Author:** Ardian Syaputra