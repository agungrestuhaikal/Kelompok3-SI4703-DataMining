# 📊 Telco Customer Churn Analysis

Proyek ini bertujuan untuk menganalisis data pelanggan dari perusahaan telekomunikasi menggunakan pendekatan **Data Mining**, khususnya melalui dua teknik utama:
- **K-Means Clustering** untuk segmentasi pelanggan (Unsupervised Learning)
- **Logistic Regression** untuk prediksi pelanggan yang berpotensi berhenti berlangganan (*churn*) (Supervised Learning)

---

## 📂 Dataset

Dataset yang digunakan adalah [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn), tersedia secara publik melalui Kaggle.

### ✨ Deskripsi Dataset
Dataset ini mencakup informasi pelanggan seperti:
- **Data demografi**: gender, umur, status pernikahan, dll.
- **Layanan yang digunakan**: internet, telepon, dukungan teknis, dll.
- **Detail kontrak**: jenis kontrak, metode pembayaran, biaya bulanan.
- **Target**: apakah pelanggan melakukan churn (`Yes`) atau tidak (`No`).

### 🔢 Contoh Fitur:
| Fitur              | Deskripsi                                         |
|--------------------|---------------------------------------------------|
| `customerID`       | ID unik tiap pelanggan                            |
| `gender`           | Jenis kelamin pelanggan                           |
| `SeniorCitizen`    | Apakah pelanggan lansia (1 = Ya, 0 = Tidak)       |
| `tenure`           | Lama berlangganan dalam bulan                     |
| `InternetService`  | Jenis layanan internet yang digunakan             |
| `Contract`         | Tipe kontrak (Month-to-month, One year, etc.)     |
| `MonthlyCharges`   | Biaya langganan bulanan                           |
| `TotalCharges`     | Total akumulasi pembayaran                        |
| `Churn`            | Target (Yes = churn, No = tidak churn)            |

---

## 📓 Jupyter Notebook

Notebook ini berisi seluruh tahapan proses analisis data, dari eksplorasi awal hingga pembuatan model dan evaluasi.

### 🔍 Struktur Analisis:
1. **Import Library**  
   Semua library Python yang dibutuhkan (pandas, numpy, matplotlib, seaborn, sklearn, imblearn, dll)

2. **Data Understanding**  
   Menampilkan struktur data, ringkasan statistik, nilai kosong, dan visualisasi awal.

3. **Data Preprocessing**  
   - Menghapus duplikat dan menangani missing value
   - Encoding fitur kategorikal (Label Encoding)
   - Normalisasi dan standarisasi data (MinMaxScaler & StandardScaler)
   - Reduksi dimensi menggunakan **PCA**

4. **Unsupervised Learning - K-Means Clustering**
   - Segmentasi pelanggan ke dalam 10 klaster
   - Evaluasi dengan **Silhouette Score**
   - Visualisasi hasil clustering (2D PCA)

5. **Supervised Learning - Logistic Regression**
   - Prediksi churn pelanggan
   - Penyeimbangan data menggunakan **SMOTE**
   - Evaluasi dengan metrik: **Accuracy, Precision, Recall, F1 Score, ROC AUC**
   - Visualisasi Kurva ROC

6. **Model Deployment (Opsional)**
   - Penyimpanan model dan pipeline preprocessing dalam format `.pkl`
   - Simulasi input data baru

---

## 🗃️ Struktur File


---

## 🧠 Insight Utama

### ✅ Logistic Regression:
- Accuracy: **76.30%**
- Precision: **74.49%**
- Recall: **79.45%**
- F1 Score: **76.89%**
- ROC AUC: **0.8409**

### 🔹 K-Means Clustering (K = 10):
- Silhouette Score: **0.3461** (clustering sedang, dapat ditingkatkan)

---

## 👨‍💻 Tim Pengembang
- Muhammad Fadli Deandri Putra  
- Andi Meuthia Rionawita  
- Frixtho Alex Credorius Latumahina  
- Agung Restu Haikal  

---

## 📄 Lisensi
Proyek ini bersifat open-source dan hanya digunakan untuk keperluan pembelajaran dan tugas akademik.

