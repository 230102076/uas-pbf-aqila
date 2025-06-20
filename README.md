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

Menggunakan Http::get() dari Laravel HTTP Client untuk mengambil data pasien & obat dari backend:

Copy
Edit
$response = Http::get('http://localhost:8080/pasien');
$dataPasien = $response->json()['data'];
CRUD Pasien & Obat
Tiap entitas punya controller tersendiri (PasienController, ObatController) yang berisi method index, create, store, edit, update, destroy.

View disusun rapi dalam folder resources/views/pasien dan resources/views/obat, dan dirender melalui Blade templating engine.

Fitur Pencarian
Fungsi index() memiliki logika pencarian sederhana yang memfilter data berdasarkan nama atau kategori:

php
Copy
Edit
if ($search) {
    $dataObat = array_filter($dataObat, function ($obat) use ($search) {
        return str_contains(strtolower($obat['nama_obat']), $search);
    });
}


