# Tugas Pertemuan 11 - CONTROLLER, VIEW, & BLADE COMPONENT (MVC PATTERN)

**Nama:** Isnaeni Kholifatun
**NIM:** 60324075
**Prodi:** Informatika
**Semester:** 4
**Repository:** []

---

## Tugas 1 : Membuat halaman dashboard yang menampilkan ringkasan statistik perpustakaan.

**Perintah yang dijalankan:**
* Contoroller Buat `DashboardController` dengan method `index()` `php artisan make:controller DashboardController`
* Menambahkan route `dashboard`
* Membuat view dashboard
* Menampilkan statistik buku dan anggota

**Data yang Ditampilkan:**
* Total buku
* Buku tersedia
* Buku habis
* Total anggota
* Anggota aktif
* Anggota nonaktif
* List 5 buku terbaru
* 5 anggota terbaru

#### 1. Dokumentasi Tugas
![1.Controller](screenshots-makecontrollerdashboard.png)
![2.TampilanDataDashboard](screenshots-dashboard.jpeg)

---

## Tugas 2 : Membuat Blade Component reusable untuk menampilkan card buku.

**Perintah yang dijalankan:**
* Generate Component`php artisan make:component BukuCard`
* Mengatur Component Properties (`$buku` dan `$showActions`)
* Mendesain layout card di `buku-card.blade.php`

**Spesifikasi Card:**
* Menampilkan: Icon cover, judul, pengarang, harga, dan stok
* Badge kategori (Programming, Database, dll)
* Status ketersediaan (Tersedia/Habis)
* Tombol aksi (Detail & Edit) bersifat kondisional

**Dokumentasi Tugas 2:**
![1.Generate Component](screenshots-makecomponentbukucard.png)
![2.Blade Component Buku Card](screenshots-bladecomponentbukucard.jpeg)

---

## Tugas 3 : Menambahkan fitur pencarian dan filter advanced untuk buku.

**Perintah yang dijalankan:**
* Membuat method `search` pada `BukuController`
* Menambahkan route `/buku/search`
* Membuat form filter pada view index buku

**Fitur Search & Filter:**
* Input keyword (search judul, pengarang, penerbit)
* Filter kategori (dropdown)
* Filter tahun (dropdown)
* Filter ketersediaan (Semua/Tersedia/Habis)

**Controller Method:**
* `public function search(Request $request)
{
    $query = Buku::query();
    
    // Filter implementation
    
    $bukus = $query->latest()->get();
    return view('buku.index', compact('bukus'));
}`

**Dokumentasi Tugas 3:**
![1.Form Search BUku](screenshots-formsearch.png)
![2.Pencarian Berdasarkan Judul `Modern Web Design`](screenshots.searchjudulpng)
![3.Hasil Pencarian Judul](screenshots-hasilpencarian.png)

