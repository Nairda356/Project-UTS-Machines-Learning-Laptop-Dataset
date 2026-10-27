# Project UTS Machine Learning
## Klasifikasi Laptop Menggunakan Algoritma Support Vector Machine (SVM)

Project ini dibuat untuk memenuhi tugas Ujian Tengah Semester (UTS) mata kuliah **Machine Learning**. Tujuannya adalah membangun model yang mengelompokkan laptop ke dalam tiga kategori berdasarkan harga dan spesifikasinya, yaitu **Entry Level**, **Mid Level**, dan **High End**.

## Deskripsi Project

Dataset laptop diolah terlebih dahulu agar atribut spesifikasinya dapat digunakan oleh algoritma machine learning. Setelah kategori dibuat, model Support Vector Machine (SVM) dilatih dan dievaluasi menggunakan data pengujian.

## Dataset

- **Nama file:** `laptop.csv`
- **Ukuran dataset awal:** 3.976 baris dan 18 kolom
- **Atribut yang tersedia antara lain:** merek, harga, prosesor, RAM, GPU, SSD, HDD, dan ukuran layar.

> File `laptop.csv` harus tersedia di folder yang sama dengan notebook agar dapat dibaca oleh program.

## Kategori Laptop

Model menggunakan tiga label klasifikasi:

- **Entry Level** — laptop untuk kebutuhan dasar.
- **Mid Level** — laptop untuk kebutuhan menengah.
- **High End** — laptop dengan spesifikasi atau harga yang relatif tinggi.

Label kategori dibuat melalui aturan berdasarkan harga, RAM, GPU, dan karakteristik prosesor tertentu. Aturan ini merupakan asumsi untuk kebutuhan project, bukan standar resmi pengelompokan laptop.

## Tahapan Pengerjaan

1. **Import library** — menggunakan Pandas, NumPy, Matplotlib, Seaborn, dan Scikit-learn.
2. **Membaca dataset** — memuat `laptop.csv` dan melihat struktur awal data.
3. **Memeriksa data** — memeriksa tipe data, statistik, dan nilai kosong.
4. **Membersihkan data** — menghapus duplikasi, mengolah atribut spesifikasi menjadi numerik, dan menangani data yang tidak valid.
5. **Membuat label** — menentukan kategori Entry Level, Mid Level, dan High End.
6. **Visualisasi kategori** — melihat distribusi data pada setiap kategori.
7. **Preprocessing** — menangani nilai kosong, melakukan penskalaan fitur numerik, dan mengubah fitur kategorikal menjadi format numerik.
8. **Membagi dataset** — memisahkan data menjadi data latih dan data uji.
9. **Melatih model** — menggunakan algoritma SVM dengan kernel RBF.
10. **Evaluasi model** — menilai hasil menggunakan accuracy, classification report, dan confusion matrix.
11. **Visualisasi hasil** — menampilkan perbandingan kategori aktual dengan hasil prediksi serta visualisasi evaluasi.
12. **Prediksi kategori** — menguji model untuk memprediksi kategori laptop.

## Teknologi dan Library

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Cara Menjalankan

1. Pastikan Python dan Jupyter Notebook sudah terpasang.
2. Simpan file `laptop.csv` dan notebook project dalam folder yang sama.
3. Instal library yang diperlukan jika belum tersedia:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. Buka Jupyter Notebook, lalu buka file notebook project.
5. Jalankan setiap cell secara berurutan dari atas hingga bawah.

## Hasil Evaluasi

Pada hasil eksekusi notebook yang disertakan, model memperoleh **akurasi 88,82%** pada data pengujian. Nilai ini menunjukkan seberapa sering prediksi model sesuai dengan label kategori yang dibuat dalam dataset.

Hasil classification report pada eksekusi tersebut:

| Kategori | Precision | Recall | F1-score |
|---|---:|---:|---:|
| Entry Level | 0,88 | 0,90 | 0,89 |
| Mid Level | 0,83 | 0,80 | 0,82 |
| High End | 0,95 | 0,95 | 0,95 |

Hasil dapat berbeda jika dataset atau pengaturan model diubah.

## Catatan

Kategori target dalam project ini dibuat menggunakan aturan berdasarkan atribut laptop, kemudian dipelajari oleh model SVM. Oleh karena itu, nilai evaluasi menunjukkan kemampuan model mempelajari aturan label tersebut dan tidak secara langsung membuktikan bahwa kategori yang dihasilkan merupakan penilaian resmi atau mutlak terhadap kelas laptop di dunia nyata.

## Struktur File

```text
Project-UTS-MachineLearning/
├── README.md
├── Project_UTS_MachineLearning.ipynb
└── laptop.csv
```

*Nama file notebook pada struktur di atas dapat disesuaikan dengan nama file yang digunakan di repository.*

## Penulis

**Nama:** Adrian Majid Saktiawan  
**Mata Kuliah:** Machine Learning  
**Jenis Tugas:** Ujian Tengah Semester (UTS)

## Referensi
**1. MAE, MSE, dan R2**
- Hodson (2022). Root-mean-square error (RMSE) or mean absolute error (MAE): when to use them or not. Geoscientific Model Development, 15, 5481-5487. (Artikel jurnal)
Link: https://gmd.copernicus.org/articles/15/5481/2022/
- Detecting heterogeneity parameters and hybrid models for precision farming. Journal of Big Data (2023). (Artikel jurnal)
Link: https://journalofbigdata.springeropen.com/articles/10.1186/s40537-023-00810-8/tables/2
**2. Jenis Data, Ukuran Dataset, Linearitas**
- Chimwanda et al. (2025). Linear Regression in the Spotlight: From Statistical Staple to... Journal of Technological Sciences, 2(1). (Artikel jurnal)
Link: https://journals.cut.ac.zw/index.php/jts/article/download/363/89/1277
