# Laravel 11 API - Belajar dari SantriKoding

Proyek ini adalah hasil pembelajaran membangun RESTful API menggunakan Laravel 11, mengikuti tutorial dari [SantriKoding](https://santrikoding.com).

## Fitur
- RESTful API dasar (CRUD)
- Respons JSON terstandarisasi dengan Resource Laravel
- (Tambahkan fitur lain sesuai dengan apa yang sudah dipelajari)

## Persyaratan
- PHP >= 8.2
- Composer
- MySQL atau database lain yang didukung Laravel

## Cara Menjalankan Proyek Secara Lokal

1. Kloning repositori ini:
   ```bash
   git clone <url-repositori-anda>
   ```

2. Masuk ke direktori proyek:
   ```bash
   cd laravel11-api
   ```

3. Instal dependensi PHP menggunakan Composer:
   ```bash
   composer install
   ```

4. Salin file konfigurasi environment:
   ```bash
   cp .env.example .env
   ```

5. Hasilkan *application key*:
   ```bash
   php artisan key:generate
   ```

6. Konfigurasi database Anda di dalam file `.env` (misalnya DB_DATABASE, DB_USERNAME, DB_PASSWORD).

7. Jalankan migrasi database:
   ```bash
   php artisan migrate
   ```

8. Mulai server pengembangan lokal:
   ```bash
   php artisan serve
   ```

API sekarang dapat diakses di `http://localhost:8000`.
