# Klasifikasi Data dengan Backpropagation Neural Network & FN-GLVQ

Proyek ini merupakan implementasi dan evaluasi metode klasifikasi menggunakan **Backpropagation Neural Network (BPNN)** dan **Fuzzy-Neuro Generalized Learning Vector Quantization (FN-GLVQ)** pada dataset `DATASE_1.csv`.

## Dataset
- **Nama file**: `DATASE_1.csv`
- Dataset ini berisi data yang digunakan untuk proses klasifikasi.
- Fitur dan target klasifikasi dijelaskan pada bagian preprocessing di notebook/source code.

## Tujuan
1. Mengembangkan dan mengimplementasikan model klasifikasi berbasis kecerdasan buatan.
2. Membandingkan performa fungsi aktivasi **Sigmoid** dan **Tanh** pada model BPNN.
3. Mengevaluasi efektivitas model **FN-GLVQ** terhadap data dengan distribusi non-linear.
4. Menganalisis performa model berdasarkan metrik seperti akurasi, recall, specificity, dan F1-Score.

## ⚙Metode yang Digunakan

### 1. Backpropagation Neural Network (BPNN)
- Digunakan dua fungsi aktivasi:
  - **Sigmoid**
  - **Tanh**
- Proses pelatihan dilakukan menggunakan algoritma **backpropagation**.
- Model diuji menggunakan metrik evaluasi seperti akurasi dan F1-score.

### 2. Fuzzy-Neuro Generalized Learning Vector Quantization (FN-GLVQ)
- Menggabungkan metode **fuzzy logic** dan **neural learning vector quantization**.
- Lebih fleksibel untuk menangani data non-linear dan memiliki toleransi terhadap noise.

## Hasil Evaluasi

| Model        | Aktivasi | Akurasi  | Precision | Recall (Sensitivity) | F1-Measure | Specificity | Waktu Training  | Waktu Testing   |
|--------------|----------|----------|-----------|----------------------|------------|-------------|------------------|------------------|
| BPNN         | Sigmoid  | 0.9787   | 0.9884    | 0.9899               | 0.9892     | 0.4242      | 3.0751 detik     | 0.0029 detik     |
| BPNN         | Tanh     | 0.9802   | 0.9802    | 1.0000               | 0.9900     | 0.0000      | 2.9981 detik     | 0.0007 detik     |
| FN-GLVQ      | -        | 0.7827   | -         | 0.6442               | 0.4800     | 0.5000      | 16.8022 detik    | 0.1118 detik     |


## Teknologi dan Library
- Python 3.x
- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Scikit-learn](https://scikit-learn.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)

## Kesimpulan
- Fungsi aktivasi **Tanh** memberikan hasil terbaik pada model BPNN dalam hal akurasi dan F1-score.
- FN-GLVQ memiliki waktu pelatihan yang lebih lama dan akurasi yang lebih rendah, namun masih relevan untuk kasus tertentu yang membutuhkan pendekatan fuzzy.
- Evaluasi model menunjukkan pentingnya pemilihan arsitektur dan fungsi aktivasi yang sesuai dengan karakteristik data.

## Catatan tambahan
Proyek ini sepenuhnya dikerjakan secara from scratch, tanpa menggunakan framework deep learning seperti TensorFlow atau PyTorch. Seluruh algoritma, termasuk Backpropagation Neural Network dan FN-GLVQ, diimplementasikan langsung menggunakan logika dasar dan library fundamental seperti NumPy dan Pandas.
Hal ini dilakukan untuk:
1. Memahami mekanisme inti dari setiap algoritma.

2. Melatih kemampuan dalam merancang dan mengimplementasikan model kecerdasan buatan dari nol.

3. Menunjukkan bahwa pembelajaran mesin tidak selalu bergantung pada library besar, tetapi dapat dibangun sendiri selama memahami konsep dasarnya.

"Proyek ini dibangun dari awal untuk mendalami konsep dasar algoritma. Segala saran dan masukan sangat dihargai untuk pengembangan lebih lanjut."


