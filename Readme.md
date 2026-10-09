# Portofolio Personal | Farel Bayuputra Irawan

Halaman portofolio / resume digital untuk **Tugas 1 Pemrograman Web** (Semester Ganjil TA 2026/2027).
Dibangun murni dengan **HTML5** dan **CSS3**, tanpa framework CSS (Bootstrap, Tailwind, dan sejenisnya) dan tanpa JavaScript.

## Tentang

Mahasiswa Teknik Informatika angkatan 2024, Universitas Muhammadiyah Malang, dengan minat di jaringan komputer dan keamanan siber. Tampilan halaman bertema *network / terminal* untuk menggambarkan bidang minat tersebut.

## Struktur Berkas

```
Portofolio/
├── index.html   # struktur dan konten halaman
├── style.css    # seluruh gaya dan layout
├── foto.jpg     # foto profil
└── README.md    # dokumentasi ini
```

## Cara Menjalankan

1. Pastikan keempat berkas berada di **satu folder yang sama**.
2. Buka `index.html` dengan browser (klik dua kali, atau klik kanan lalu *Open with*).
3. Opsional: di VS Code, pasang ekstensi **Live Server** supaya halaman refresh otomatis saat berkas disimpan.

Tidak perlu instalasi apa pun. Font dimuat dari Google Fonts, sehingga butuh koneksi internet. Tanpa internet, halaman tetap tampil dengan font bawaan sistem.

## Bagian Halaman

| Bagian | Isi |
| --- | --- |
| Hero | Nama, peran, foto profil, dan diagram topologi jaringan |
| Tentang saya | Ringkasan diri dan bidang minat |
| Pendidikan | UMM (Teknik Informatika) dan SMAN 1 Besuki |
| Keahlian | Jaringan, aplikasi, data, dan infrastruktur |
| Proyek | GameHub (Laravel + Oracle XE 21c di Docker) |
| Pengalaman organisasi | KKN |
| Kontak | Email, GitHub, LinkedIn, Instagram |

## Penerapan Kriteria Penilaian

### Struktur dan semantik HTML
- Tag semantik: `header`, `nav`, `main`, `section`, `article`, `figure`, `address`, `footer`.
- Hirarki heading berurutan: satu `h1`, lalu `h2` per bagian, lalu `h3` per entri.
- `lang="id"`, `meta viewport`, `meta description`, dan `alt` pada gambar.
- Setiap `section` terhubung ke judulnya lewat `aria-labelledby`, plus tautan *skip to content*.
- Data berpasangan memakai `dl`, `dt`, dan `dd`; tanggal memakai `time`.

### Penerapan CSS dan layouting
- Satu berkas `style.css` yang terbagi dalam bagian bernomor dan berkomentar.
- Warna, font, dan jarak dipusatkan di *design tokens* (CSS variables) pada `:root`.
- Flexbox untuk navbar dan chip, CSS Grid untuk hero, kartu, dan statistik.
- Navbar *glassmorphism* di atas tengah (`backdrop-filter`) dengan cadangan untuk browser yang belum mendukung.
- Penanda menu aktif murni CSS lewat `scroll-target-group` dan `:target-current`.

### Responsivitas
- Pendekatan *mobile-first* dengan dua breakpoint: **640px** (tablet) dan **960px** (desktop).
- Hero satu kolom di mobile dan dua kolom di desktop.
- Navbar bisa digeser horizontal di layar sempit.
- Animasi dimatikan otomatis untuk pengguna dengan pengaturan `prefers-reduced-motion`.

## Catatan Kompatibilitas

- Penanda menu aktif (`:target-current`) saat ini berjalan di browser berbasis Chromium (Chrome, Edge, Brave). Di browser lain, menu tetap berfungsi normal tanpa penanda tersebut.
- Efek blur navbar membutuhkan dukungan `backdrop-filter`; jika tidak ada, navbar memakai latar solid.

## Validasi

HTML dapat diperiksa di [validator.w3.org](https://validator.w3.org/) lewat tab *Validate by File Upload*.

## Teknologi

HTML5, CSS3, Google Fonts (JetBrains Mono dan IBM Plex Sans).

## Penulis

**Farel Bayuputra Irawan**
Teknik Informatika, Universitas Muhammadiyah Malang