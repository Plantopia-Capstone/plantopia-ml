# Plantopia-ML – Deteksi Penyakit Tanaman Berbasis Deep Learning

> Sistem deteksi penyakit tanaman berbasis citra daun menggunakan model deep learning dengan arsitektur CNN.  
> Dibuat sebagai bagian dari **Capstone Project** tema _Environment & Sustainability_ – Coding Camp 2025.

---

## Tentang Kami

Repositori ini adalah dokumentasi lengkap dari proyek `Plantopia-ML`, solusi AI untuk membantu masyarakat mengenali penyakit tanaman secara otomatis hanya dari gambar daun.

---

## Daftar Isi

- [Latar Belakang](#-latar-belakang)
- [Tujuan Proyek](#-tujuan-proyek)
- [Struktur Folder](#-struktur-folder)
- [Model dan Arsitektur](#-model-dan-arsitektur)
- [Evaluasi Model](#-evaluasi-model)
- [Cara Menjalankan](#-cara-menjalankan)
- [Tim Pengembang](#-tim-pengembang)
- [Lisensi](#-lisensi)

---

## Latar Belakang

Penyakit tanaman merupakan salah satu penyebab utama menurunnya produktivitas pertanian.  
Sayangnya, tidak semua petani memiliki akses terhadap tenaga ahli untuk diagnosis penyakit secara cepat dan akurat.

**Plantopia-ML hadir sebagai solusi berbasis AI** yang dapat melakukan deteksi penyakit tanaman hanya dari gambar daun, memanfaatkan kekuatan _computer vision_ dan _deep learning_.

---

## Tujuan Proyek

- Mengembangkan model klasifikasi penyakit tanaman berbasis citra daun.
- Meningkatkan kesadaran teknologi AI di bidang pertanian dan keberlanjutan.
- Memberikan solusi praktis, cepat, dan akurat bagi petani, pelajar, dan masyarakat umum.

---

## Struktur Folder

```
plantopia-ml/
│
├── models/                # Model .h5 hasil pelatihan
├── notebooks/             # Notebook eksplorasi, preprocessing, dan pelatihan model
├── assets/                # Visualisasi, rating, atau aset tambahan
├── app.py                 # Script Gradio untuk demo model
├── requirements.txt       # Dependensi Python
└── README.md              # Dokumentasi ini
```

---

## Model dan Arsitektur

Model utama yang digunakan:
- ✅ **CNN (Convolutional Neural Network)** – pretrained dan fine-tuned dengan transfer learning.
- ✅ **MobileNetV2** – digunakan karena ringan dan cepat, cocok untuk deployment di web dan perangkat edge.
- ✅ Augmentasi & preprocessing gambar: `ImageDataGenerator`, `rescale`, `flip`, `zoom`, dsb.

---

## Evaluasi Model

| Metrik            | Nilai                                |
|-------------------|--------------------------------------|
| Akurasi Validasi  | 96%+                                 |
| Akurasi Uji       | Tergantung subset penyakit (94–97%)  |
| Confusion Matrix  | ✅ Diuji terhadap noise & outlier     |
| Prediksi Gradio   | ✅ [Plantopia Hub](https://huggingface.co/spaces/sulthonkaf/plantopia-hub) |

---

## Cara Menjalankan

1. **Clone repo:**

```bash
git clone https://github.com/Plantopia-Capstone/plantopia-ml.git
cd plantopia-ml
```

2. **Install dependencies:**

```bash
pip install -r requirements.txt
```

3. **Jalankan demo Gradio:**

```bash
python app.py
```

4. **Buka di browser**: `http://localhost:7860`

---

## Tim Pengembang

| Nama                          | Peran                      | Institusi                           | Kode Peserta              |
|-------------------------------|----------------------------|-------------------------------------|---------------------------|
| Sulthon Kaffaah Al Farizzi    | Machine Learning Developer | Universitas Muhammadiyah Surakarta  | (ML) MC268D5Y2007         |
| Fitria Irfani Mutashim        | Machine Learning Developer | Universitas Gadjah Mada             | (ML) MC008D5X1800         |
| Gabriella Yoanda Pelawi       | Machine Learning Developer | Universitas Gadjah Mada             | (ML) MC008D5X2466         |

---

## Lisensi

Proyek ini dirilis dengan lisensi **MIT License** – silakan gunakan, kontribusikan, atau fork untuk inovasi lanjutan dengan tetap menjaga etika open-source.

---

> “Inovasi yang bermakna tumbuh dari akar kepedulian dan semangat berbagi.”  
> — *Plantopia Team* 
