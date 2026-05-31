# Tugas Pertemuan 11 - CONTROLLER, VIEW, & BLADE COMPONENT (MVC PATTERN)

**Identitas Mahasiswa:**
**Nama:** Isnaeni Kholifatun
**NIM:** 60324075
**Prodi:** Informatika
**Semester:** 4
**Mata Kuliah:** Pemrograman Web II
**Repository:** [https://github.com/isnaenikholifatun/Pertemuan11-CONTROLLER-VIEW-MVC-PATTERN-/tree/main/tugas-praktikum11]

---

## 📊 Tugas 1: Dashboard Statistik Perpustakaan

**Langkah-langkah dan Perintah:**
1. Membuat Controller `DashboardController`: `php artisan make:controller DashboardController`.
2. Menambahkan route `dashboard` pada file `web.php`.
3. Membuat view dashboard untuk menampilkan ringkasan data.
4. Menampilkan statistik utama:
    * Total buku, Buku tersedia, dan Buku habis.
    * Total anggota, Anggota aktif, dan Anggota nonaktif.
    * Daftar 5 buku terbaru & 5 anggota terbaru.

**Dokumentasi Tugas 1:**
1. ![1.Controller](screenshots/makecontrollerdashboard.png)
2. ![2.TampilanDataDashboard](screenshots/dashboard.jpeg)

---

## 🧩 Tugas 2: Blade Component Reusable (Card Buku)

**Langkah-langkah dan Perintah:**
1. Generate Component: `php artisan make:component BukuCard`.
2. Mengatur Component Properties seperti `$buku` dan `$showActions`.
3. Mendesain layout kartu buku di `buku-card.blade.php`.
4. Implementasi fitur:
    * Menampilkan Cover, Judul, Pengarang, Harga, dan Stok.
    * Badge kategori otomatis (Programming, Database, dll).
    * Status ketersediaan (Tersedia/Habis).
    * Tombol aksi kondisional (Detail & Edit).

**Dokumentasi Tugas 2:**
1. ![1.Generate Component](screenshots/makecomponentbukucard.png)
2. ![2.Blade Component Buku Card](screenshots/bladecomponentbukucard.jpeg)

---

## 🔍 Tugas 3: Fitur Pencarian & Filter Advanced

**Langkah-langkah dan Perintah:**
1. Membuat method `search` pada `BukuController`.
2. Menambahkan route `/buku/search`.
3. Membuat form filter pada view index buku.
4. Fitur Filter mencakup:
    * Keyword (Judul, Pengarang, Penerbit).
    * Dropdown Kategori dan Tahun.
    * Filter Status Ketersediaan.

**Dokumentasi Tugas 3:**
1. ![1.Form Search Buku](screenshots/formsearch.png)
2. ![2.Pencarian Berdasarkan Judul](screenshots/searchjudul.png)
3. ![3.Hasil Pencarian Judul](screenshots/hasilpencarian.png)