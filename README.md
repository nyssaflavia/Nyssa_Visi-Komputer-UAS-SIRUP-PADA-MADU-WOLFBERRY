# 🍯 Wolfberry Honey Adulteration Detector 🔬

Aplikasi berbasis web interaktif ini dirancang untuk mengidentifikasi adulterasi (pemalsuan) sirup pada madu wolfberry menggunakan data spektrum **¹H Nuclear Magnetic Resonance (¹H NMR)**. Sistem mengintegrasikan arsitektur **Convolutional Neural Network (CNN)** yang dipadukan dengan **Convolutional Block Attention Module (CBAM)** sebagai mekanisme perhatian (attention mechanism), serta **Support Vector Machine (SVM)** sebagai classifier akhir untuk menghasilkan deteksi yang akurat dan andal.

---

# 🚀 Demo Aplikasi (Online)

Aplikasi telah dideploy secara cloud dan dapat diakses melalui:

👉 **https://your-streamlit-app.streamlit.app**

*(Ganti dengan link Streamlit Anda setelah deployment.)*

---

# 🌟 Fitur Utama

### 🧪 Analisis Spektrum ¹H NMR
Menganalisis data spektroskopi ¹H NMR untuk mengenali karakteristik kimia madu wolfberry dan mendeteksi indikasi adulterasi sirup.

### 🧠 Model CNN-CBAM-SVM
Menggunakan kombinasi arsitektur **CNN**, **CBAM**, dan **SVM** untuk memperoleh representasi fitur yang lebih informatif sehingga meningkatkan akurasi klasifikasi.

### 📂 Upload Data Mudah
Mendukung unggah data spektrum dalam format yang telah disediakan sehingga pengguna dapat melakukan identifikasi secara cepat.

### ⚡ Prediksi Cepat
Memberikan hasil klasifikasi hanya dalam beberapa detik dengan tingkat akurasi yang tinggi.

### 📊 Visualisasi Hasil
Menampilkan hasil prediksi, tingkat keyakinan (confidence score), serta kategori sampel yang teridentifikasi.

### 📖 Informasi Edukatif
Memberikan penjelasan mengenai adulterasi madu, manfaat analisis ¹H NMR, serta interpretasi hasil prediksi.

---

# 🛠️ Prasyarat Sistem

Pastikan perangkat Anda telah terpasang:

- Python 3.9 – 3.11
- Git
- pip

---

# 📦 Instalasi

## 1. Clone Repository

```bash
git clone https://github.com/username/Wolfberry-Honey-Adulteration-Detector.git

cd Wolfberry-Honey-Adulteration-Detector
```

## 2. Membuat Virtual Environment (Opsional)

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🖥️ Menjalankan Aplikasi

```bash
streamlit run app.py
```

Setelah berhasil dijalankan, aplikasi dapat diakses melalui:

👉 **http://localhost:8501**

---

# 📂 Struktur Proyek

```
├── app.py
├── requirements.txt
├── model/
│   ├── cnn_cbam_svm.pkl
│   ├── scaler.pkl
│   └── label_encoder.pkl
├── dataset/
├── assets/
├── pages/
└── README.md
```

---

# 🔬 Metodologi

Alur kerja sistem terdiri dari beberapa tahapan:

1. Akuisisi data spektrum ¹H NMR.
2. Pra-pemrosesan data spektrum.
3. Ekstraksi fitur menggunakan CNN.
4. Peningkatan representasi fitur menggunakan CBAM.
5. Klasifikasi menggunakan Support Vector Machine (SVM).
6. Menampilkan hasil identifikasi adulterasi.

---

# 📊 Output Sistem

Sistem akan memberikan informasi berupa:

- Status sampel:
  - ✅ Madu Wolfberry Murni
  - ⚠️ Madu Wolfberry Teradulterasi Sirup

- Confidence Score (%)

- Probabilitas setiap kelas

- Visualisasi hasil prediksi

---

# 🎯 Tujuan Penelitian

Penelitian ini bertujuan mengembangkan sistem identifikasi adulterasi sirup pada madu wolfberry berbasis kecerdasan buatan yang memanfaatkan data spektroskopi **¹H NMR**. Dengan menggabungkan CNN, CBAM, dan SVM, sistem diharapkan mampu meningkatkan akurasi deteksi sehingga dapat mendukung pengawasan kualitas madu, membantu industri pangan, serta melindungi konsumen dari produk madu yang dipalsukan.

---

# 📚 Referensi

Jika Anda menggunakan proyek ini dalam penelitian, mohon sitasi publikasi terkait.

Contoh:

> **Implementasi CNN-CBAM-SVM untuk Identifikasi Adulterasi Sirup pada Madu Wolfberry Berbasis Spektroskopi ¹H NMR.**

*(Tambahkan informasi jurnal setelah penelitian dipublikasikan.)*

---

# 👨‍💻 Teknologi yang Digunakan

- Python
- Streamlit
- TensorFlow / Keras
- Scikit-Learn
- NumPy
- Pandas
- Matplotlib
- Plotly

---

# 📝 Lisensi

Proyek ini dilisensikan di bawah **MIT License**.

Silakan lihat file **LICENSE** untuk informasi lebih lanjut.
