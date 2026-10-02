# Telkom University Company Profile - Praktikum

Project simulasi HTML, CSS, PHP native, MySQL/MariaDB, dan Git.

Project ini adalah simulasi website company profile sederhana yang dibangun untuk memenuhi tugas praktikum Pemrograman Web. Website ini menggunakan PHP native, MySQL/MariaDB, dan dikelola versinya menggunakan Git.

## Fitur Utama
* **Beranda:** Halaman utama yang dapat diakses tanpa error PHP.
* **Program Studi:** Menampilkan data program studi yang diambil langsung dari database.
* **Berita:** Fitur list berita dan halaman detail berita yang berfungsi penuh.
* **Kontak:** Form kontak yang dapat menyimpan pesan pengguna ke dalam database.
* **Admin Lokal:** Fitur simulasi untuk menambah berita baru.

## Persyaratan Sistem
* Web Server Lokal Laragon
* PHP 7.4 atau lebih baru
* MySQL / MariaDB
* Git

## Riwayat Praktikum Git
* 17e2eb7 (HEAD -> main, tag: v1.0.0, origin/main) message : cara menjalankan project ini
* 077e653 feat: membalikan Profile
* 71da9b5 Revert "feat: ubah label profil jadi Tentang Ayos"
* 6e5a57b feat: tambahkan catatan dari laptop A
* 922a7de feat: tambahkan catatan dari laptop B
*   a53f487 merge: selesaikan conflict navbar
|\  
| * 1872b6d (conflict-navbar) feat: ubah label profil jadi Tentang Ayos
* | c32fe8a style: ubah label profil di main
* | b23660b feat: ubah label profil di branch simulasi
* | 749764a style: ubah label profil pada main
|/  
* 87dbdfd feat: ubah label profil pada branch conflict
* da49ec1 feat: tambahkan informasi fokus pembelajaran
* e9f194e feat: tambahkan form admin lokal untuk berita
* a2678c3 feat: simpan pesan kontak ke database
* c68f6ea feat: tambahkan daftar dan detail berita
* c97a7ac feat: hubungkan database dan tampilkan program studi
* f89838e feat: update profil halaman
* 176dc5f feat: tambahkan layout dasar dan stylesheet
* bb005e7 chore : inisialisasi project dan dokumentasi awal

## Penjelasan Merge Conflict
Simulasi merge conflict dilakukan dengan mengubah baris teks yang sama persis pada file `includes/header.php` di dua branch berbeda, yaitu `main` dan `conflict-navbar`. Karena kedua branch mengubah titik yang sama, Git menolak penggabungan otomatis dan menandai file sebagai konflik dengan marker `<<<<<<<`, `=======`, dan `>>>>>>>`. 

Penyelesaiannya dilakukan dengan:
1. Memilih teks final secara manual di file yang konflik
2. Menghapus semua marker konflik
3. Menjalankan `git add includes/header.php`
4. Menjalankan `git commit -m "merge: selesaikan conflict navbar"`

Setelah merge selesai, branch `conflict-navbar` dihapus karena sudah tidak diperlukan lagi.

## Cara Menjalankan Project

1. **Clone Repository**
   Buka terminal dan jalankan perintah berikut:
   ```bash
   git clone https://github.com/FarrosAbhista/telkom-company-profile-109062500012.git
   ```

2. **Pindahkan Folder**
   Pindahkan folder hasil clone ke dalam direktori web server lokal
    `D:\laragon\www\`.

3. **Impor Database**
   Buka phpMyAdmin, buat database baru, lalu impor file SQL yang ada di dalam folder `database/` project ini.

4. **Konfigurasi Koneksi Database**
   Buka file `config/database.php`. Sesuaikan nama database, username, dan password dengan konfigurasinya.

5. **Akses Website**
   Buka browser dan akses alamat lokal kamu, misalnya:
   `http://localhost/telkom-company-profile-109062500012/`