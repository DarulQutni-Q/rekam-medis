# Rekam Medis

Aplikasi web sederhana untuk sistem rekam medis rumah sakit dengan CRUD
sederhana (mata kuliah Sistem Basis Data). Mengelola data pasien dan
rekam medisnya.

## Tech Stack

- PHP (MySQLi), tanpa framework
- MySQL / MariaDB
- CSS polos (`style.css`, `pasien_style.css`)

## Cara Menjalankan

1. Buat database dan impor strukturnya. `koneksi.php` akan otomatis
   mengimpor `create_db.sql` saat pertama kali terhubung kalau database
   `db_rekammedis` belum ada.
2. Sesuaikan kredensial database di `koneksi.php` kalau perlu
   (default: host `127.0.0.1`, user `root`, password kosong,
   database `db_rekammedis`).
3. Jalankan server lokal dari folder proyek:

```bash
php -S localhost:8000
```

4. Buka http://localhost:8000. Halaman utama mengalihkan ke aplikasi
   di folder `app/`.

## Struktur File

- `index.php` — pengalihan ke aplikasi di `app/`
- `app/` — aplikasi rekam medis (hasil rebuild)
- `koneksi.php` — koneksi MySQL (otomatis impor `create_db.sql` kalau perlu)
- `create_db.sql` — struktur database `db_rekammedis`
- `style.css`, `pasien_style.css` — stylesheet
