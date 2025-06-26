# Deteksi Plat Nomor Kendaraan dengan YOLO
Proyek ini adalah implementasi model object detection untuk mendeteksi plat nomor kendaraan secara real-time dari gambar. Proyek ini dibangun sebagai bagian dari tugas Ujian Akhir Semester (UAS) Machine Learning, dengan model yang dilatih menggunakan arsitektur YOLO (You Only Look Once).

# Fitur Utama
Deteksi Akurat: Model dilatih pada dataset kustom untuk mengenali plat nomor dengan berbagai kondisi pencahayaan dan sudut.

Konfigurasi Mudah: Menggunakan file data.yaml untuk manajemen dataset yang terstruktur.

Ekstensibel: Kode dan struktur proyek dirancang agar mudah dikembangkan atau dilatih ulang dengan dataset yang berbeda.

Eksperimen di Notebook: Dilengkapi dengan file Jupyter Notebook (.ipynb) untuk analisis dan pengujian model.

# Panduan Instalasi dan Penggunaan
Ikuti langkah-langkah berikut untuk menjalankan proyek ini di komputer lokal Anda.

1. Persiapan Awal
Salin repositori ini ke mesin lokal Anda menggunakan git.

git clone [https://github.com/rofusedcryof/Machine-Learning.git] https://github.com/rofusedcryof/Machine-Learning.git
cd UAS

1. Setup Virtual Environment
Sangat disarankan untuk membuat virtual environment agar dependensi proyek tidak tercampur dengan proyek lain.

# Untuk Windows
python -m venv venv
.\venv\Scripts\activate

# Untuk macOS/Linux
python3 -m venv venv
source venv/bin/activate

3. Instalasi Dependensi
Install semua library yang dibutuhkan menggunakan pip. Anda disarankan untuk membuat file requirements.txt terlebih dahulu.

pip install -r requirements.txt

Contoh requirements.txt:

torch
torchvision
opencv-python
numpy
pyyaml
matplotlib

4. Menjalankan Deteksi
Gunakan skrip detect.py untuk melakukan inferensi pada gambar. Pastikan Anda sudah memiliki file bobot model (.pt).

# Ganti 'path/to/your/image.jpg' dengan lokasi gambar Anda
# Ganti 'path/to/your/best.pt' dengan lokasi file bobot model Anda
python detect.py --source "path/to/your/image.jpg" --weights "path/to/your/best.pt"

Hasil deteksi akan disimpan secara otomatis di direktori runs/detect/exp.

📁 Struktur Direktori Proyek
UAS/
├── 📄 235314023-235314036.ipynb   # Notebook utama untuk eksperimen
├── 📄 data.yaml                     # Konfigurasi dataset untuk YOLO
├── 📁 labels/                       # Anotasi (bounding box) untuk dataset
│   ├── 📁 train/
│   └── 📁 val/
├── 📁 images/                       # Gambar asli untuk dataset (jika ada)
│   ├── 📁 train/
│   └── 📁 val/
└── 📄 detect.py                     # Skrip untuk menjalankan deteksi (jika ada)

📄 Lisensi
Proyek ini dilisensikan di bawah Lisensi MIT. Lihat file LICENSE untuk informasi lebih lanjut.

🧑‍💻 Kontak
Dibuat oleh Dionysius Diaz Damar Wilansa

Dionysius Diaz Damar Wilansa: 
# LinkedIn: https://www.linkedin.com/in/dionysius-diaz-damar-wilansa-934843336/
# GitHub  : https://github.com/rofusedcryof
# Email   : dezttroll@gmail.com
