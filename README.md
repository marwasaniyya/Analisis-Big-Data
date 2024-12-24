# **Tugas Akhir: Analisis Big Data**

## Daftar Isi
- [Tentang](#tentang)
- [Diagram Alur Proses](#diagram-alur-proses)
- [Dependensi](#dependensi)
- [Tim](#tim)

---

## Tentang
Proyek ini bertujuan untuk memberikan pemahaman mendalam terkait pola status reservasi hotel, termasuk kategori "Canceled" dan "Not Canceled." Analisis ini bertujuan untuk mengidentifikasi pola musiman, tren pembatalan, serta ketidakhadiran tamu, yang dapat mendukung pengambilan keputusan strategis dalam industri perhotelan.

Sebagai bagian dari proyek ini, sebuah Storyboard telah dibuat untuk menyajikan gambaran visual tentang alur analisis dan temuan utama. **Tautan Storyboard**: [Klik di sini untuk melihat Storyboard](https://prezi.com/view/or0p7VqRZAChL9Og6skY/). Proyek ini memanfaatkan Python dan pustaka visualisasi data untuk menghasilkan grafik yang interaktif dan informatif. File utama proyek ini berupa Jupyter Notebook yang menyajikan analisis data secara terperinci, mulai dari tahap persiapan data hingga visualisasi hasil.

---

## Diagram Alur Proses

![Analisis drawio]![Diagram Tanpa Judul drawio](https://github.com/user-attachments/assets/27500814-b93f-4c80-855a-f3a6d3373d27)


### Penjelasan Diagram  

1. **Dataset**  
   Analisis dimulai dengan dataset utama, yaitu `Hotels.csv`, yang berisi informasi tentang status reservasi hotel. Dataset ini mencakup beberapa fitur penting seperti tanggal reservasi, durasi menginap, jenis kamar, jumlah tamu, dan status reservasi (Canceled atau Not Canceled).  

2. **Pra-Pemrosesan Data**  
   Tahapan pra-pemrosesan mencakup beberapa langkah berikut:  
- **Penanganan Nilai NAN:** Dataset dibersihkan dengan menghapus baris atau kolom yang mengandung banyak nilai kosong (NAN) atau menggantinya dengan nilai tertentu, seperti rata-rata untuk data numerik.  
- **Eliminasi Kolom:** Kolom `country` dihapus dari dataset.  
- **Transformasi Data:** Kolom tertentu, seperti tanggal, dikonversi ke format datetime untuk mempermudah analisis berbasis waktu. Kolom kategorikal diubah menjadi bentuk numerik melalui metode seperti one-hot encoding atau label encoding.  
- **Normalisasi Data:** Data numerik dinormalisasi ke dalam rentang tertentu untuk meningkatkan kinerja model.   

3. **Visualisasi Data**  
   Data yang telah melalui tahap pra-pemrosesan divisualisasikan menggunakan diagram histogram, yang membantu menggambarkan distribusi dan pola dari data secara lebih jelas dan informatif.

4. **Pemodelan Random Forest**  
   Model Random Forest diterapkan untuk mengklasifikasikan status reservasi, dengan langkah-langkah berikut:  
- Memisahkan dataset menjadi data pelatihan dan data pengujian.  
- Melatih model pada data pelatihan menggunakan hyperparameter yang telah dioptimalkan.  
- Mengevaluasi kinerja model menggunakan metrik seperti akurasi, precision, recall, dan F1-score.  
5. **Rangkuman**  
  Proyek ini disimpulkan dengan merangkum temuan utama dari analisis, meliputi:  
- Penentuan fitur-fitur utama yang berpengaruh terhadap status pembatalan reservasi.  
- Wawasan mengenai pola musiman dan tren pembatalan.  
- Rekomendasi strategis untuk pengelola hotel, seperti pengoptimalan strategi reservasi atau promosi berdasarkan hasil analisis.  
---

## Dependensi
- `Tensorflow` >= 2.17.1
- `Panda` >= 2.2.2
- `Numpy` >= 1.26.4
- `Matplotlib.Pyplot` >= 3.8.0
- `Seaborn` >= 0.13.2
- `Sklearn Pandas` >= 2.2.0
- `Scikit-Learn` >= 1.6.0
- `python` >= 3.10 

Untuk informasi lebih lanjut, lihat file `requirements.txt` di repositori ini.

---

## Tim
- 👨‍💻 [Saniyya Ruzzy Marwa](https://github.com/marwasaniyya)
- 👨‍💻 [Rezandy Kusbiantoro Nurul Mubin](https://github.com/Rezandy16)
- 👨‍💻 [M. Syauqi Aalaikar Rahman](https://github.com/syauqiAlaik)

## Terima Kasih
