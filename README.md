# 🐔🐶🕷️ Animal Classification
Proyek ini bertujuan untuk membangun model deep learning yang dapat mengklasifikasikan gambar hewan: ayam (chicken), anjing (dog), dan laba-laba (spider).

# 🙌 Dataset
Dataset diperoleh dari Kaggle [Animals-10](https://www.kaggle.com/datasets/alessiocorrado99/animals10)

# 🚀 Cara Penggunaan
Pelatihan Ulang Model:
Buka dan jalankan notebook train_model.ipynb untuk melatih ulang model.

Pengujian Model:
Jalankan inference.ipynb untuk melakukan prediksi terhadap gambar baru.

Deployment:
Gunakan file .tflite untuk aplikasi mobile atau folder tfjs_model/ untuk aplikasi web.

# 🔥 Ringkasan Pelatihan
- Proporsi dataset: 70% train / 15% validation / 15% test
- Ukuran input gambar: 128x128 piksel
- Arsitektur CNN:
- 4x Conv2D + BatchNormalization + MaxPooling
- GlobalAveragePooling
- Fully Connected Layer
- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Evaluasi: Accuracy

# 📂 Struktur Direktori
 ```
submission
├───tfjs_model
| ├───group1-shard1of1.bin
| └───model.json
├───tflite
| ├───model.tflite
| └───label.txt
├───saved_model
| ├───saved_model.pb
| └───variables
├───notebook.ipynb
├───README.md
└───requirements.txt
 ```