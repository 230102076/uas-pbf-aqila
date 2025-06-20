<h1> Sistem Informasi Rumah Sakit <h1>
Deskripsi
Repositori ini merupakan hasil pengerjaan Ujian Akhir Semester Mata Kuliah Praktikum Pemrograman Berbasis Framework Semester Genap Tahun Ajaran 2024/2025.
Sistem ini dibuat menggunakan Laravel untuk frontend dan CodeIgniter 4 untuk backend, dengan studi kasus pengelolaan data pasien dan obat pada rumah sakit.

Fitur Utama
CRUD data pasien

CRUD data obat

Pencarian data pasien dan obat

Konsumsi REST API dari backend (CodeIgniter 4) menggunakan HTTP Client Laravel

Validasi form dan alert error

Tampilan responsif sederhana

Instalasi & Menjalankan Proyek
🔧 Backend
Clone repository backend dari:
https://github.com/abdau88/uas_pbf_soal_A.git

Jalankan perintah berikut:

bash
Copy
Edit
composer install
php spark serve
Import file SQL dan ubah nama database menjadi db_rumahsakit_[NIM_ANDA]

🌐 Frontend
Clone repository ini

Jalankan:

bash
Copy
Edit
composer install
npm install && npm run dev
php artisan serve
Pastikan koneksi ke backend sesuai (localhost:8080)

Tambahan (Opsional)
Jika tersedia:

Fitur export data ke PDF/Excel

Upload gambar pasien

Simulasi login sederhana

Error handling dari API dengan alert
