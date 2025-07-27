# Proyek Klasifikasi Gambar Pokémon

Proyek ini mengimplementasikan model klasifikasi gambar menggunakan **TensorFlow** dan **Keras** untuk mengklasifikasikan gambar Pokémon berdasarkan tipe mereka (misalnya: Air, Petir). Proyek ini disusun sebagai bagian dari submisi oleh **Hilmi Datu Allam**.


Model klasifikasi dirancang untuk mengenali tipe Pokémon melalui gambar. Proyek mencakup:

- Pemuatan dan pra-pemrosesan dataset
- Pembangunan dan pelatihan CNN (Convolutional Neural Network)
- Evaluasi model terhadap data uji

---

## 📁 Dataset

Dataset digunakan untuk melatih model klasifikasi gambar Pokémon berdasarkan **tipe utama** seperti:

- `Water`
- `Fire`
- `Grass`
- `Lightning` (Electric)
- `Psychic`
- `Rock`
- `Ground`
- dan lain-lain

Dataset bersumber dari [Kaggle](https://www.kaggle.com/ltihium123/pokemon-dataset) 

## 🧠 Detail Model

- **Arsitektur:** CNN dengan layer `Conv2D`, `MaxPooling2D`, `Dropout`, `BatchNormalization`, dan `Dense`
- **Input:** Gambar dipotong (kanan atas), diubah ukurannya ke `48x34 piksel`, dan dinormalisasi ke [0, 1]
- **Output:** Prediksi label tipe Pokémon dengan skor kepercayaan
