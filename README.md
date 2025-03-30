# Machine-Learning-for-Bank-Transaction-Analysis

## 📝 Overview
> Pada proyek ini, saya mengembangkan model Machine Learning dengan dua pendekatan utama:
> Supervised Learning: Menggunakan klasifikasi untuk mengelompokkan data berdasarkan label yang telah ditentukan sebelumnya.
> Unsupervised Learning: Menerapkan clustering untuk menemukan pola dalam data tanpa label tertentu.
> Tujuan utama dari proyek ini adalah untuk menganalisis pola perilaku pelanggan dalam transaksi bank dan membantu pengambilan keputusan strategis dalam layanan perbankan.

## 📌 Dataset dan Metodologi
Dataset yang digunakan mencakup berbagai transaksi perbankan, termasuk informasi pelanggan, jenis transaksi, serta jumlah transaksi.
### 🔍 Langkah-Langkah:
#### Clustering (Unsupervised Learning)
> Menggunakan algoritma K-Means untuk membagi pelanggan ke dalam beberapa kelompok berdasarkan karakteristik transaksi mereka.
#### Klasifikasi (Supervised Learning)
> Setelah cluster terbentuk, data digunakan untuk membangun model klasifikasi guna memprediksi segmen pelanggan baru.

## 🔎 Hasil Clustering dengan K-Means
Berdasarkan hasil clustering menggunakan metode K-Means, pelanggan dapat dikelompokkan ke dalam dua kategori utama:
```
> Cluster 0: Pelanggan yang lebih tua, profesional (dokter/insinyur), dengan saldo akun tinggi dan kebiasaan transaksi rutin melalui ATM.
> Cluster 1: Pelanggan muda, mayoritas pelajar, dengan saldo akun lebih rendah tetapi aktif bertransaksi secara online di berbagai platform.
```
Wawasan ini membantu bank dalam menyesuaikan strategi layanan berdasarkan preferensi dan kebiasaan pelanggan.

📊 Evaluasi Model Klasifikasi
Beberapa model diuji untuk mengklasifikasikan pelanggan berdasarkan cluster yang telah terbentuk, dengan hasil sebagai berikut:
### ✅ Random Forest (Model Terbaik)
```
> Akurasi sebelum tuning: 99.13%
> Akurasi setelah tuning: 98.91%
> Precision kelas 0 turun dari 99% ke 98%, tetapi recall kelas 0 meningkat dari 99% ke 100%.
> Precision kelas 1 naik dari 99% ke 100%, tetapi recall kelas 1 turun dari 98% ke 96%.
> Perbedaan akurasi training-testing berkurang dari 0.54% menjadi 0.06%, menunjukkan peningkatan generalisasi.
```

### 🔹 Decision Tree
```
> Akurasi sebelum tuning: 98.91%
> Akurasi setelah tuning: 98.91% (stabil).
> Precision dan recall tetap stabil untuk kedua kelas (precision kelas 0: 99%, recall kelas 0: 99%, precision kelas 1: 98%, recall kelas 1: 99%).
> Tuning tidak mengubah performa secara signifikan tetapi mempertahankan stabilitas model.
```

### 🔹 Logistic Regression
```
> Akurasi sebelum tuning: 98.48%
> Akurasi setelah tuning: 98.70%
> Precision kelas 0 tetap 99%, recall kelas 0 meningkat dari 98% ke 99%.
> Precision kelas 1 tetap 97%, recall kelas 1 tetap stabil di 99%.
> Tidak ada indikasi overfitting atau underfitting; model generalisasi dengan baik.
```


## 🎯 Kesimpulan
Random Forest terbukti menjadi model terbaik dalam mengelompokkan pelanggan berdasarkan transaksi mereka.
Model ini memiliki keseimbangan akurasi yang baik, tahan terhadap overfitting, dan mampu menangkap pola kompleks dalam data transaksi bank.
Wawasan yang diperoleh dari clustering dapat digunakan untuk meningkatkan strategi layanan perbankan dan personalisasi produk bagi pelanggan.
💡 Proyek ini menunjukkan bagaimana Machine Learning dapat dimanfaatkan dalam dunia keuangan untuk memahami pelanggan dengan lebih baik dan meningkatkan layanan perbankan secara efisien.
