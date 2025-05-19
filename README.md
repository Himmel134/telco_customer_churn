# Customer Churn Prediction – Telco Dataset

Proyek ini bertujuan untuk membangun model prediksi churn pelanggan menggunakan machine learning, dengan fokus utama pada efisiensi biaya retensi. Proyek ini menyasar tim Churn Retention agar dapat mengidentifikasi pelanggan berisiko tinggi dan melakukan intervensi secara lebih tepat sasaran.

---

## File Struktur

- `data_telco_customer_churn.csv`  
  Dataset utama berisi informasi pelanggan seperti durasi langganan, jenis layanan, dan status churn.

- `notebook_churn.ipynb`  
  Notebook analisis yang berisi:
  - Exploratory Data Analysis (EDA)
  - Preprocessing (encoding, scaling)
  - Model building & benchmarking
  - Threshold tuning
  - Evaluasi berbasis metrik bisnis (cost-based)

- `Presentation.pptx`  
  Presentasi akhir berisi ringkasan temuan, visualisasi, dan rekomendasi strategis untuk tim bisnis.

---

## Tujuan Proyek

- Memprediksi pelanggan yang berisiko churn menggunakan data historis.
- Mengoptimalkan strategi retensi agar lebih hemat biaya.
- Memberikan insight bagi tim bisnis melalui interpretasi model (feature importance & SHAP).
- Menyediakan threshold optimal berdasarkan biaya retensi dan potensi kehilangan pelanggan.

---

## Model dan Evaluasi

- Model utama: **Logistic Regression**
- Teknik balancing: **SMOTE**
- Metrik utama: **ROC AUC**, **Recall**, **Precision**
- Threshold tuning untuk memaksimalkan recall (mencegah false negative) dengan mempertimbangkan total biaya.

---

## Hasil Utama

- Recall meningkat dari 0.55 → 0.84 dengan threshold tuning dan SMOTE.
- Biaya retensi dapat ditekan dari Rp77 juta → Rp58 juta berdasarkan simulasi bisnis.
- Fitur paling berpengaruh: `tenure`, `MonthlyCharges`, dan `InternetService`.

---

## Rekomendasi

- Fokus intervensi pada pelanggan dengan probabilitas churn > 0.8.
- Gunakan hasil model sebagai daftar prioritas mingguan bagi tim Retention.
- Evaluasi hasil intervensi secara berkala dan lakukan pengembangan model lebih lanjut.

---

## 📌 Sumber Data

Dataset diambil dari:  
[Google Drive – Telco Churn Data](https://drive.google.com/drive/folders/1_fR7R0srpZgnFnanbrmELgnK-xmzMAHp?usp=drive_link)

