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
> Memiliki precision dan recall yang tinggi.
> Perbedaan akurasi training-testing berkurang dari 0.54% menjadi 0.06%, menunjukkan peningkatan generalisasi.
```

### 🔹 Decision Tree
```
> Lebih rentan terhadap overfitting meskipun memiliki interpretabilitas tinggi.
```

### 🔹 Logistic Regression
```
> Efektif untuk data dengan pola linear tetapi kurang optimal dalam menangani kompleksitas pola transaksi.
```


## 🎯 Kesimpulan
Random Forest terbukti menjadi model terbaik dalam mengelompokkan pelanggan berdasarkan transaksi mereka.
Model ini memiliki keseimbangan akurasi yang baik, tahan terhadap overfitting, dan mampu menangkap pola kompleks dalam data transaksi bank.
Wawasan yang diperoleh dari clustering dapat digunakan untuk meningkatkan strategi layanan perbankan dan personalisasi produk bagi pelanggan.
💡 Proyek ini menunjukkan bagaimana Machine Learning dapat dimanfaatkan dalam dunia keuangan untuk memahami pelanggan dengan lebih baik dan meningkatkan layanan perbankan secara efisien.
