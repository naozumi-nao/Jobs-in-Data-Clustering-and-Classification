# Data Clustering dan Classification

Repository ini berisi proyek akhir untuk kelas Belajar Machine Learning untuk Pemula di Dicoding. Proyek ini menunjukkan implementasi dan evaluasi berbagai algoritma clustering dan klasifikasi data.

## Sumber Dataset
https://www.kaggle.com/datasets/hummaamqaasim/jobs-in-data/

## Gambaran Proyek

Proyek ini bertujuan untuk mendemonstrasikan pemahaman praktis dan penerapan konsep dasar machine learning, khususnya di bidang:

* **Clustering Data:** Mengelompokkan titik data yang serupa.
* **Klasifikasi Data:** Mengkategorikan titik data ke dalam kelas yang telah ditentukan sebelumnya.

## Isi Repository

* `[Clustering].ipynb`: Berisi implementasi dan evaluasi clustering.
* `[Klasifikasi].ipynb`: Berisi implementasi dan evaluasi klasifikasi.
* `jobs_in_data.csv`: Berisi dataset asli.
* `jobs_in_data_after_clustering.ipynb`: Berisi dataset setelah dilakukan preprocessing dan clustering.
* `README.md`: File ini.
* `requirements.txt`: Daftar library Python yang diperlukan untuk menjalankan notebook.

## Setup

1.  Clone repository ini:
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2.  Buat virtual environment (disarankan):
    ```bash
    python -m venv venv
    source venv/bin/activate # Di Linux/macOS
    venv\Scripts\activate # Di Windows
    ```

3.  Install library yang diperlukan:
    ```bash
    pip install -r requirements.txt
    ```

4.  Buka dan jalankan Jupyter Notebook di direktori `notebooks/`.

## Library yang Digunakan

* `pandas`: Untuk manipulasi data dalam bentuk DataFrame.
* `numpy`: Untuk operasi numerik dan array.
* `matplotlib`: Untuk visualisasi data dasar.
* `seaborn`: Untuk visualisasi data yang lebih interaktif dan estetis.
* `math`: Untuk operasi matematika dasar.
* `sklearn.metrics`:
    * `silhouette_score`: Untuk mengevaluasi kualitas clustering dengan silhouette score.
    * `confusion_matrix`: Untuk evaluasi performa model klasifikasi.
    * `accuracy_score`, `precision_score`, `recall_score`, `f1_score`: Untuk metrik evaluasi klasifikasi.
    * `classification_report`: Untuk laporan klasifikasi yang lebih detail.
* `sklearn.preprocessing`:
    * `MinMaxScaler`: Untuk normalisasi data.
    * `LabelEncoder`: Untuk encoding variabel kategori.
* `sklearn.cluster`:
    * `KMeans`: Untuk metode clustering KMeans.
    * `DBSCAN`: Untuk metode clustering DBSCAN.
* `sklearn.neighbors`: `NearestNeighbors` untuk mencari tetangga terdekat, digunakan dalam DBSCAN.
* `sklearn.decomposition`: `PCA` untuk reduksi dimensi menggunakan Principal Component Analysis (PCA).
* `os`: Untuk operasi sistem seperti mengatur variabel lingkungan.
* `warnings`: Untuk mengelola peringatan agar tidak mengganggu output.
* `sklearn.model_selection`:
    * `train_test_split`: Untuk membagi data menjadi set pelatihan dan pengujian.
    * `learning_curve`: Untuk visualisasi performa model terhadap ukuran data pelatihan.
    * `BayesSearchCV`: Untuk optimasi hiperparameter dengan pencarian Bayesian.
* `sklearn.tree`: `DecisionTreeClassifier` untuk model klasifikasi Decision Tree.
* `sklearn.ensemble`: `RandomForestClassifier` untuk model klasifikasi Random Forest.
* `imblearn.over_sampling`: `SMOTE` untuk menangani ketidakseimbangan kelas dengan oversampling.