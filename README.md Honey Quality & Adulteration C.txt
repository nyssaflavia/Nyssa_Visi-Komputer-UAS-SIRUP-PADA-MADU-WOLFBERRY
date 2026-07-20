# 🍯 Honey Quality & Adulteration Classifier (CNN-CBAM-SVM) 🔍

Aplikasi berbasis web interaktif ini dirancang untuk memprediksi **kemurnian dan pemalsuan (adulterasi) madu** secara instan berbasis citra spektrum $^1\text{H}$ **NMR (Nuclear Magnetic Resonance)**. Sistem ini mengintegrasikan ekstraktor fitur mendalam **CNN-CBAM** (*Convolutional Neural Network* dengan *Convolutional Block Attention Module*) dan klasifikasi tingkat lanjut berbasis **SVM** (*Support Vector Machine*) untuk analisis kualitas madu yang presisi dan andal.

---

## 🚀 Demo Aplikasi (Online)

Aplikasi ini telah di-deploy secara cloud dan dapat diakses secara publik melalui tautan berikut:
👉 **[klasifikasi-madu-cbam.gradio.live](https://gradio.app)** *(Atau tautan Hugging Face Spaces Anda)*

---

## 🌟 Fitur Utama

* **Atensi Ganda Spasial & Channel (CBAM):** Memfokuskan ekstraksi fitur secara otomatis pada area puncak spektrum $^1\text{H}$ NMR yang paling relevan dengan molekul gula dan bahan adulterasi.
* **Pengklasifikasi Hybrid High-Precision (SVM):** Menggabungkan representasi fitur *Deep Learning* dengan ketegasan *hyperplane* pembatas margin optimal khas SVM.
* **Analisis & Diagnostik Instan:** Mengolah citra spektrum dan menampilkan hasil prediksi (*Madu Murni* vs *Madu Palsu*) hanya dalam waktu $\approx 0.5$ detik.
* **Metode Input Fleksibel:** Mendukung berbagai format pengunggahan berkas citra spektrum (`.jpg`, `.jpeg`, `.png`) dengan proses otomatis *resize* dan *scaling*.
* **Antarmuka Interaktif Gradio:** Menyajikan antarmuka pengguna berbasis web yang bersih, ramah pengguna, serta dilengkapi skor tingkat kepastian (*confidence score*).

---

## 📂 Penjelasan Detail Struktur Berkas

Agar sistem dapat memuat model dan menjalankan antarmuka tanpa kendala di lingkungan lokal, pastikan seluruh berkas berikut berada dalam satu direktori kerja:

```text
├── requirements.txt                 # Daftar pustaka & dependensi Python
├── app.py                           # Kode utama aplikasi & antarmuka Gradio
├── cnn_cbam_feature_extractor.h5    # Model ekstraktor fitur terlatih CNN-CBAM
├── svm_model.pkl                    # Model pengklasifikasi terkalibrasi SVM
├── scaler.pkl                       # Objek pemrosesan normalisasi fitur (StandardScaler)
└── README.md                        # Dokumentasi teknis & panduan proyek