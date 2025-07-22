# 🏁 Tugas Akhir (TA) - Final Project

**Nama Mahasiswa**: Muhammad Naufal Baihaqi  
**NRP**: 5025211103  
**Judul TA**: Pembuatan Data Sintetik 
pada Data Histori Pasien Menggunakan Metode Berbasis GAN untuk Deteksi Risiko 
Komplikasi Terapi CAPD  
**Dosen Pembimbing**: Dini Adni Navastara, S.Kom., M.Sc.  
**Dosen Ko-pembimbing**: Prof. Dr. Eng. Chastine Fatichah, 
S.Kom., M.Kom.

---

## 📺 Demo Aplikasi   

[![Demo Aplikasi](https://private-user-images.githubusercontent.com/115441787/469359411-3d49d0b9-1cf3-469e-bb0a-2638c0cbb3b7.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTMyMDQzODksIm5iZiI6MTc1MzIwNDA4OSwicGF0aCI6Ii8xMTU0NDE3ODcvNDY5MzU5NDExLTNkNDlkMGI5LTFjZjMtNDY5ZS1iYjBhLTI2MzhjMGNiYjNiNy5qcGc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNzIyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDcyMlQxNzA4MDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03MDJlNWNlN2E2Y2E3ZDU2MzM4OGFiMzI5Y2E3MjA0NWM4ZDAxZDYyMzdmN2NiNWZiZDlkNWU3OWQ4NTU5MTEyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.hZ3Z5WEYXHsFU2q_e1ybqUJ6JSe1ej7X6j7zwaj_t44)](https://youtu.be/DJT7ODeUCE0)  
*Klik gambar di atas untuk menonton demo*

---

## 🛠 Panduan Instalasi & Menjalankan Program  

### Prasyarat  
- Dataset:
   - final_data (menjalankan ipynb utama dari awal) = [link](https://drive.google.com/drive/folders/1JYM3TTH2_LtXNKMSJXiwVNp5gGe7CmyW?usp=sharing)
   - image before cropping:
      - normal = [link](https://drive.google.com/drive/folders/1u0kBhtxuOKyxT38c7uPZzhpqCmF6_ivN?usp=sharing)
      - abnormal = [link](https://drive.google.com/drive/folders/1zqSWSObN3vIkF6vd3S_lrgn6c8WT8Ife?usp=sharing
   - data raw:)
      - normal = [link](https://drive.google.com/file/d/1GM3kMMXTyOzLcaiyN4zJFnlaek5JSNXQ/view?usp=sharing)
      - abnormal = [link](https://drive.google.com/file/d/14HtZQo2XizVJ7WOP78WB9tKi88gSvugW/view?usp=sharing)
  - data bersih (jika ingin langsung memproses tanpa generate sintetik data) = [link](https://drive.google.com/drive/folders/1ZvPjHA9kbxbxwJSu_o9LMdWK83wczfBn?usp=sharing)
- Model GAN:
   - CTABGAN = [link](https://github.com/Team-TUD/CTAB-GAN) (clone lalu masukkan bagian model nya ke dalam folder)
   - CTABGAN+ = [link](https://github.com/Team-TUD/CTAB-GAN-Plus) (clone lalu masukkan bagian model nya ke dalam folder)
   - CTGAN & CopulaGAN lewat library


### Langkah-langkah  
1. **Clone Repository**  
   ```bash
   git clone https://github.com/Informatics-ITS/ta-naufalqii16.git
   ```
2. **Instalasi Dependensi**
   ```bash
   cd [folder-proyek]
   python -m venv myenv # Crete virtual environment
   .\myvenv\Scripts\activate # Activate virtual environment
   pip install -r requirements.txt  # Install dependencies
   ```
3. **Skenario**
- `1_get_data_first.ipynb` digunakan jika ingin memulai dari awal sekali (menghasilkan data raw)
- `create_bag_detection_model.ipynb` digunakan untuk membuat model pre-trained untuk cropping gambar
- `bag_detector.ipynb` digunakan untuk melakukan cropping gambar
- `2_feature_extraction.ipynb` digunakan untuk melakukan feature extraction dari data gambar yang telah di-crop
- `SDG_Modelling.ipynb` pipeline utama proses synthetic data dan modelling


---

## ✅ Validasi

Pastikan proyek memenuhi kriteria berikut sebelum submit:
- Source code dapat di-build/run tanpa error
- Video demo jelas menampilkan fitur utama
- README lengkap dan terupdate
- Tidak ada data sensitif (password, API key) yang ter-expose

---

## ⁉️ Pertanyaan?

Hubungi:
- Penulis: [naufalqii16@gmail.com]
