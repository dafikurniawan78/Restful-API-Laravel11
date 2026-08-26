<div align="center">
  <h1>🚀 Laravel 11 RESTful API</h1>
  <p><strong>Proyek Membangun RestfulAPI bersama SantriKoding</strong></p>

  <p>
    <a href="https://laravel.com/"><img src="https://img.shields.io/badge/Laravel-11.x-FF2D20?style=for-the-badge&logo=laravel" alt="Laravel 11"/></a>
    <a href="https://php.net/"><img src="https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php" alt="PHP 8.2"/></a>
    <a href="https://santrikoding.com/"><img src="https://img.shields.io/badge/Tutorial-SantriKoding-00B4D8?style=for-the-badge" alt="SantriKoding"/></a>
  </p>
</div>

<hr/>

## 📖 Tentang Proyek

Repositori ini adalah hasil dari proses pembelajaran langkah demi langkah dalam membangun **RESTful API** menggunakan framework **Laravel 11**. Tutorial ini bersumber dari [SantriKoding](https://santrikoding.com), platform belajar coding berbahasa Indonesia. 

Tujuan utama dari proyek ini adalah untuk memahami konsep dasar pembuatan API, mulai dari desain database, pengelolaan model, hingga mengembalikan response dalam format JSON yang terstandarisasi (menggunakan `API Resource`).

---

## ✨ Fitur Utama (On Progress)

Karena proyek ini sedang dalam tahap pengembangan (mengikuti seri tutorial), berikut adalah fitur-fitur yang direncanakan dan sudah diimplementasikan:

- [x] **Setup & Konfigurasi** Laravel 11
- [x] **Model & Migration** untuk entitas `Post`
- [x] **API Resource** (`PostResource`) untuk format JSON response yang konsisten
- [ ] **Create (POST)**: Endpoint untuk menambahkan data artikel beserta unggah gambar
- [ ] **Read (GET)**: Endpoint untuk menampilkan semua data dan data spesifik
- [ ] **Update (PUT/PATCH)**: Endpoint untuk memperbarui data
- [ ] **Delete (DELETE)**: Endpoint untuk menghapus data

---

## 🛠️ Teknologi yang Digunakan

* **Framework:** [Laravel 11](https://laravel.com/)
* **Bahasa Pemrograman:** [PHP 8.2+](https://www.php.net/)
* **Database:** MySQL / MariaDB
* **Format Response:** JSON

---

## 🚀 Panduan Instalasi Lokal

Ingin mencoba menjalankan API ini di komputer Anda sendiri? Ikuti langkah-langkah mudah di bawah ini:

### 1. Kloning Repositori
```bash
git clone https://github.com/username-anda/nama-repositori.git
cd nama-repositori
```

### 2. Instalasi Dependensi
Pastikan Anda sudah menginstal **Composer** di sistem Anda.
```bash
composer install
```

### 3. Konfigurasi Environment
Salin file `.env.example` menjadi `.env` lalu sesuaikan konfigurasi database Anda.
```bash
cp .env.example .env
```
Gunakan teks editor untuk mengubah bagian ini pada file `.env`:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=nama_database_anda
DB_USERNAME=root
DB_PASSWORD=
```

### 4. Generate Application Key
```bash
php artisan key:generate
```

### 5. Jalankan Migrasi Database
Agar tabel `posts` dan yang lainnya dibuat secara otomatis.
```bash
php artisan migrate
```

### 6. Jalankan Server Lokal
```bash
php artisan serve
```
Voila! 🎉 API Anda sekarang dapat diakses di: `http://localhost:8000`

---

## 📂 Struktur Data Response

Proyek ini menggunakan **API Resource** (`App\Http\Resources\PostResource`) agar output JSON yang dihasilkan rapi dan profesional. Format default yang akan didapatkan pengguna API adalah sebagai berikut:

```json
{
  "success": true,
  "message": "Pesan status aksi (misal: Data Post Berhasil Ditambahkan)",
  "data": {
    "id": 1,
    "image": "http://localhost:8000/storage/posts/gambar.jpg",
    "title": "Judul Artikel",
    "content": "Isi lengkap dari artikel...",
    "created_at": "2026-08-26T10:00:00.000000Z",
    "updated_at": "2026-08-26T10:00:00.000000Z"
  }
}
```

---

## 🎓 Credit

Seluruh materi pembelajaran dan struktur dasar proyek ini mengacu pada seri tutorial luar biasa dari:
**[SantriKoding.com](https://santrikoding.com)**

> *"Teruslah belajar, karena hidup tidak pernah berhenti mengajarkan."*
