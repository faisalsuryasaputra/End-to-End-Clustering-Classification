# 🏦 Customer Segmentation & Prediction Pipeline

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Revision_Completed-green)

## 📌 Project Overview
Proyek ini mengintegrasikan pendekatan **Unsupervised** dan **Supervised Learning** untuk menganalisis perilaku nasabah perbankan. Alur kerja dimulai dengan mengelompokkan nasabah ke dalam segmen-segmen tertentu menggunakan **K-Means**, yang kemudian hasilnya digunakan sebagai label untuk melatih model klasifikasi **Random Forest**.

## 📂 Struktur Repository
Sesuai dengan ketentuan submission, repository ini berisi:
- `[Clustering]_Submission_Akhir_BMLP_Faisal_Surya_Saputra.ipynb`: Tahap EDA, Preprocessing, dan Clustering.
- `[Klasifikasi]_Submission_Akhir_BMLP_Faisal_Surya_Saputra.ipynb`: Tahap Splitting, Modeling, dan Tuning Klasifikasi.
- `model_clustering.h5`: Model K-Means yang telah dilatih.
- `PCA_model_clustering.h5`: Model clustering berbasis PCA (Advanced).
- `decision_tree_model.h5`: Model klasifikasi baseline.
- `tuning_classification.h5`: Model Random Forest yang telah di-tuning (Best Model).
- `data_clustering.csv`: Dataset hasil clustering dengan kolom label `Target`.
- `data_clustering_inverse.csv`: Dataset hasil clustering dalam format nilai asli (Inverse).

## 🛠️ Metodologi & Analisis (Kriteria 4)

### Clustering & Profiling Nasabah
Berdasarkan hasil analisis agregasi (mean, min, max) pada data yang telah di-inverse, nasabah dikelompokkan menjadi 3 segmen utama:

1.  **Cluster 0 (Young Students - Charlotte):** Nasabah muda (rata-rata 44.8 tahun) dengan profesi pelajar. Memiliki saldo rata-rata terendah namun aktif menggunakan layanan cabang.
2.  **Cluster 1 (Active Students - Tucson):** Kelompok pelajar yang sangat aktif secara transaksional dengan rata-rata nominal transaksi tertinggi (258.21).
3.  **Cluster 2 (Affluent Engineers - Fort Worth):** Segmen dewasa mapan dengan profesi Engineer. Memiliki saldo akun tertinggi (5170.92), mencerminkan profil nasabah *affluent*.



### Klasifikasi & Optimasi
Label yang dihasilkan dari clustering (`Target`) digunakan untuk melatih model klasifikasi. Model **Random Forest** yang telah di-optimasi menggunakan `GridSearchCV` berhasil mencapai akurasi **99%**, memberikan hasil prediksi yang sangat stabil untuk segmentasi nasabah baru.

## 💻 Cara Menjalankan
1. Clone repository ini.
2. Pastikan library `pandas`, `scikit-learn`, `seaborn`, dan `joblib` sudah terinstall.
3. Jalankan notebook Clustering terlebih dahulu untuk menghasilkan file dataset berlabel.
4. Jalankan notebook Klasifikasi untuk melatih dan mengevaluasi model prediksi.

## 👤 Author
**Faisal Surya Saputra**
*Informatics Student at Telkom University*
[LinkedIn](https://www.linkedin.com/in/faisalsuryasaputra/) | [GitHub](https://github.com/faisalsuryasaputra)
