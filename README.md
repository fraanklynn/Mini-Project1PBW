# Website Portofolio - Franklyn Galvin Lodo

## Tampilan Section 
1. Home (Hero Section)
  - Menampilkan navbar (Home, About Me, Certificates)
  - Menampilkan judul perkenalan + deskripsi singkat
  - Menampilkan tombol navigasi (“Tentang Saya” & “Lihat Sertifikat”)
  - Menampilkan foto profil berbentuk lingkaran dengan border
###### <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/54cfa376-59ca-40e5-9387-1795ab826089" />

2. About Me
   - Card/box “About Me” (glass effect)
   - Deskripsi diri (2 paragraf)
   - Skills menggunakan progress bar (MySQL & Python)
   - Pengalaman menggunakan list
###### <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0e1521a2-15f5-4f7f-8848-6767968021ec" />

3. Certificates
   - Menampilkan 1 sertifikat dalam card + gambar sertifikat
   - Ada judul sertifikat dan keterangan penerbit + tahun
###### <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/35b30a9a-8697-49f0-bd4d-0aac4abffbaa" />

## Penjelasan Code Setiap Section/Fitur

### 1. Navbar (```index.html```)
  - Menggunakan komponen Bootstrap navbar dengan ```class navbar-expand-lg dan fixed-top```.
  - Berisi nama portfolio dan menu navigasi:
    - Home
    - About Me
    - Certificates
  - Setiap menu menggunakan anchor link menuju section dengan id terkait (```#home, #about, #certificates```).
  - Class ```fixed-top``` membuat navbar tetap berada di atas saat halaman di-scroll.

### 2. Hero Section (```index.html```)
  - Merupakan section utama perkenalan diri.
  - Menampilkan:
    - Nama lengkap dengan efek gradient
    - Deskripsi singkat sebagai mahasiswa Sistem Informasi
    - Tombol navigasi ke About Me dan Certificates
    - Foto profil berbentuk lingkaran
  - Layout menggunakan Bootstrap Grid (```container, row, col-lg-7, col-lg-5```) untuk membagi teks dan gambar.

### 3. About Me Section (```index.html```)
  - Berisi deskripsi latar belakang pendidikan, minat, dan aktivitas organisasi.
  - Section dibungkus dengan about-box untuk membuat tampilan card transparan (glass effect).
  - Menampilkan:
    - Dua paragraf deskripsi diri
    - Skills menggunakan progress bar
    - Pengalaman dalam bentuk daftar (list)

### 4. Skills Feature (```index.html```)
  - Setiap skill menggunakan komponen Bootstrap progress dan progress-bar.
  - Persentase kemampuan ditampilkan melalui:
    - Lebar bar (```style="width: ...%"```)
    - Angka persentase di bagian atas bar
  - Skill yang ditampilkan:
    - MySQL (80%)
    - Python (60%)

### 5. Experience Feature (```index.html```)
  - Berupa daftar (```<ul><li>```) pengalaman organisasi dan proyek.
  - Isi pengalaman meliputi:
    - Perancangan ERD dan struktur database
    - Staff Human Resources Development – INFORSA (2025)
    - Lead Cadre Development Division – INFORSA (2026)

### 6. Certificates Section (```index.html```)
  - Menampilkan sertifikat menggunakan komponen Bootstrap card.
  - Komponen card terdiri dari:
    - Gambar sertifikat
    - Judul sertifikat (MySQL Database Fundamentals)
    - Nama penyelenggara dan tahun (Dicoding – 2025)
  - Layout menggunakan Bootstrap Grid agar card berada di tengah dan tetap responsif.

## Penjelasan CSS (```style.css```)

### 1. Global Style
  - ```body```:
    - Mengatur background menggunakan gradient hijau gelap
    - Mengatur font menggunakan Google Font (Poppins)
    - Memberikan padding-top untuk menyesuaikan navbar fixed

### 2. Navbar Style
  - ```.custom-navbar```:
    - Background transparan dengan efek blur
    - Border bawah tipis berwarna hijau
    - Shadow agar navbar terlihat lebih tegas
  - ```.navbar-nav .nav-link:hover:```
    - Mengubah warna menu menjadi hijau saat hover
   
### 3. Hero Style
  - ```#home:```
    - Mengatur ukuran font judul dan deskripsi
    - Memberikan efek glow pada background menggunakan pseudo-element ```::before```
  - ```.highlight-name:```
    - Memberikan efek teks gradient pada nama
  - ```.profile-img:```
    - Membuat foto berbentuk lingkaran
    - Menambahkan border dan shadow
    - Memberikan efek hover scale

### 4. About Style
  - ```.about-box:```
    - Membuat efek glassmorphism (background transparan + blur)
    - Border tipis dan border-radius
  - ```.about-text:```
    - Mengatur warna teks dan line-height agar nyaman dibaca
   
### 5. Skills Style
  - ```.progress:```
    - Mengatur tinggi dan bentuk rounded pada progress bar
  - ```.progress-mysql:```
    - Memberikan warna gradient orange
  - ```.progress-python:```
    - Memberikan warna gradient biru

### 6. Certificates Style
  - ```.card dan custom styling:```
    - Menyesuaikan background card agar sesuai dengan tema
    - Mengatur padding dan shadow
    - Mengatur ukuran gambar sertifikat agar proporsional

## Teknologi yang Digunakan
  - HTML
  - CSS
  - Bootstrap 5
