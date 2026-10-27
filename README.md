# GoedangKita

GoedangKita adalah aplikasi manajemen gudang berbasis web. Aplikasi ini dibuat sebagai tugas besar mata kuliah IPPL. Pengguna dapat mengelola data master barang, mencatat barang masuk dan barang keluar, dan mencetak laporan stok. Hak akses diatur per peran melalui menu dan submenu.

## Fitur

- Login admin dengan pembatasan akses berdasarkan peran pengguna
- Dashboard ringkasan data gudang
- Kelola jenis barang, satuan, dan merk
- Kelola data barang dan data customer
- Pencatatan transaksi barang masuk
- Pencatatan transaksi barang keluar
- Laporan stok barang, barang masuk, dan barang keluar dalam format PDF
- Kelola menu, submenu, dan hak akses peran
- Pengaturan profil pengguna dan kata sandi
- Pengaturan tampilan aplikasi

## Teknologi

- PHP 8.1
- Laravel 9
- MySQL
- Blade dan Vite
- Yajra DataTables untuk tabel data
- Dompdf untuk laporan PDF
- Laravel Sanctum

## Cara Instalasi

Prasyarat:

- PHP 8.1 atau lebih baru
- Composer
- MySQL
- Node.js dan npm

Langkah instalasi:

1. Clone repositori ini.
2. Masuk ke folder proyek lalu jalankan `composer install`.
3. Jalankan `npm install`.
4. Buat file `.env` di root proyek. Isi konfigurasi dasar seperti `APP_NAME`, `APP_KEY`, dan koneksi database `DB_CONNECTION`, `DB_HOST`, `DB_PORT`, `DB_DATABASE`, `DB_USERNAME`, `DB_PASSWORD`. Repositori ini tidak menyertakan `.env.example`, jadi file dibuat manual mengikuti format `.env` standar Laravel.
5. Jalankan `php artisan key:generate`.
6. Jalankan `php artisan migrate --seed` untuk membuat tabel dan data awal menu, peran, dan pengguna.

## Cara Menjalankan

Jalankan dua perintah berikut di terminal terpisah:

```bash
php artisan serve
npm run dev
```

Aplikasi dapat dibuka di `http://127.0.0.1:8000`. Halaman login admin berada di `/admin/login`.

Untuk build aset produksi, jalankan `npm run build`.

## Lisensi

Proyek ini memakai lisensi MIT. Lihat berkas [LICENSE](LICENSE).
