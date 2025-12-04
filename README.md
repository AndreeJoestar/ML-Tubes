# 📌 Proyek Machine Learning – Prediksi Harga Beras Surabaya 2024

Repositori ini berisi implementasi machine learning untuk memprediksi harga beras pasar Surabaya tahun 2024 menggunakan model **Random Forest Regressor** serta antarmuka **Gradio** untuk melakukan prediksi secara interaktif.

---

## 📁 **Struktur Folder & File**
Berikut penjelasan setiap file pada repositori:

| Nama File | Deskripsi |
|----------|-----------|
| **Code.ipynb** | Notebook utama yang berisi seluruh proses machine learning: import data, preprocessing, training model, evaluasi, dan visualisasi. |
| **Gradio.ipynb** | Notebook khusus untuk menjalankan aplikasi prediksi menggunakan Gradio. |
| **harga_beras_surabaya_2024.csv** | Dataset harga beras harian yang digunakan untuk training dan testing. |
| **rf_beras_surabaya_2024.joblib** | Model Random Forest yang sudah dilatih dan disimpan untuk digunakan kembali. |
| **LAPORAN PROYEK.docx** | Laporan akhir proyek machine learning. |
| **LK PERANCANGAN PROject.docx** | Dokumen perancangan awal proyek. |
| **README.md** | Dokumentasi proyek. |

---

## 🧠 **Tujuan Proyek**
Proyek ini dibuat untuk:
- Membangun model machine learning untuk **memprediksi harga beras** berdasarkan data historis.
- Menerapkan pipeline ML dari awal sampai akhir.
- Membuat aplikasi prediksi sederhana menggunakan **Gradio**.
- Memenuhi tugas besar mata kuliah Machine Learning.

---

## 📊 **Tahapan Proyek**
Tahapan yang dilakukan pada proyek ini:

### 1. **Data Loading & Cleaning**
- Membaca dataset harga beras.
- Menangani missing values.
- Membuat fitur baru seperti:
  - `day_number`
  - `month`
  - `price_lag1` (harga hari sebelumnya)

### 2. **Preprocessing**
- Encoding data waktu.
- Normalisasi fitur yang dibutuhkan.
- Split data menjadi train dan test set.

### 3. **Modeling**
Model yang digunakan:  
✔ **Random Forest Regressor**  
Dipilih karena:
- Mampu menangani data non-linear
- Akurat pada dataset time-series sederhana
- Mudah digunakan dan stabil

### 4. **Evaluasi**
Metode evaluasi:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Square Error)
- R² Score

### 5. **Deployment via Gradio**
Tersedia file **Gradio.ipynb** untuk menjalankan aplikasi prediksi.  
Input:
- Hari
- Bulan
- Harga hari sebelumnya

Output:
- Prediksi harga beras untuk hari tersebut.

---

## ▶️ **Cara Menjalankan Proyek**

### **1. Clone Repositori**
```bash
git clone https://github.com/AndreeJoestar/ML-Tubes.git
cd ML-Tubes
