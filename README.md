# Proyek Klasifikasi Gambar

## Deskripsi

Proyek ini bertujuan untuk membuat model klasifikasi gambar dengan TensorFlow. dengan target akurasi sudah mencapai bahkan melebihi 90%. Model akan diekspor ke format SavedModel, TFLite, dan TFJS.

## Struktur Folder

```
data/           -> Data latih, validasi, dan uji
notebooks/      -> Notebook Jupyter (Google Colab)
saved_model/    -> Model dalam format SavedModel
tfjs_model/     -> Model untuk web (TensorFlow.js)
tflite/         -> Model untuk mobile (TFLite)
```

## Cara Pakai

### 1. Instalasi

Pastikan semua dependensi sudah diinstal di Colab:

```python
!pip install -r requirements.txt
```

### 2. Jalankan Notebook

Semua proses pelatihan, evaluasi, dan ekspor dilakukan di dalam notebook Jupyter. Buka file notebook di folder `notebooks/` dan jalankan sel-selnya secara berurutan.

## Ekspor Model

Model sudah diekspor ke tiga format:

- **SavedModel** → di folder `saved_model/`
- **TFLite** → file `tflite/model.tflite` dan `label.txt`
- **TFJS** → file `tfjs_model/model.json` dan `.bin` untuk web
