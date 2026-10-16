# Project Screenshots

## Page 1

### Desktop

![Page 1 — Desktop](screenshot/Page-1%20desktop.png)

### Mobile

![Page 1 — Mobile](screenshot/Page-1%20mobile.png)

## Page 2

### Desktop

![Page 2 — Desktop](screenshot/Page-2%20desktop.png)

### Mobile

![Page 2 — Mobile](screenshot/Page-2%20mobile.png)

## Project Title & Status

### Mini Project Frontend: GAMIFY & Furniture Catalog

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v3.4.19-06B6D4?logo=tailwindcss&logoColor=white)
![Status](https://img.shields.io/badge/status-completed-success)

## Author

**Agung Avit**

## Deskripsi

Proyek mini ini berisi dua halaman antarmuka web yang dibuat sebagai latihan
frontend. Halaman pertama adalah landing page **GAMIFY** bertema gaming, dengan
hero, kategori produk, produk unggulan, dan bagian trending. Halaman kedua
adalah katalog furnitur untuk living room table, dilengkapi sidebar pilihan
harga, warna, material, dan ukuran, grid kartu produk, serta bagian partner
pembayaran.

> **Catatan:** Walaupun konteks tugas menyebut tema LMS, isi kode dan tangkapan
> layar yang tersedia saat ini menunjukkan landing page gaming dan katalog
> furnitur. README ini mendeskripsikan implementasi yang ada dan tidak
> mengklaim fitur LMS atau manajemen kursus.

## Teknologi

- **HTML5 semantik** untuk struktur halaman dan konten.
- **Vanilla CSS** untuk styling halaman GAMIFY di `Page-1/styles.css`.
- **Tailwind CSS 3.4** untuk styling katalog di `Page-2/src/index.html`, dengan
  konfigurasi di `Page-2/tailwind.config.js`.
- **Google Fonts:** Space Grotesk pada halaman pertama dan Poppins pada halaman
  kedua.

## Struktur Proyek

```text
.
├── Page-1/
│   ├── asset/              # Logo dan gambar untuk landing page gaming
│   ├── index.html          # Halaman landing GAMIFY
│   └── styles.css          # CSS responsif halaman pertama
├── Page-2/
│   ├── asset/              # Gambar produk, ikon, dan aset katalog
│   ├── src/
│   │   ├── index.html      # Halaman katalog furnitur
│   │   ├── input.css       # Sumber CSS dan direktif Tailwind
│   │   └── output.css      # CSS hasil kompilasi yang digunakan halaman
│   ├── package.json        # Dependensi Tailwind CSS
│   └── tailwind.config.js  # Konfigurasi Tailwind
├── screenshot/             # Screenshot desktop dan mobile
└── README.md
```

## Fitur & Implementasi

- **Dua halaman berbeda:** landing page gaming dan katalog produk furnitur.
- **Responsif:** halaman pertama memakai media query untuk breakpoint 640 px
  dan 1024 px; halaman katalog memakai utility breakpoint Tailwind seperti
  `sm:`, `md:`, dan `lg:`.
- **Layout fleksibel:** Flexbox digunakan pada navigasi, konten, serta footer;
  katalog dan kartu produknya menggunakan CSS Grid.
- **Katalog dan filter visual:** menampilkan kartu produk serta kelompok
  kontrol harga, warna, material, dan ukuran. Kontrol tersebut adalah bagian
  antarmuka; fungsionalitas penyaringan produk belum diimplementasikan.
- **Struktur konten:** halaman menggunakan elemen seperti `header`, `nav`,
  `main`, `section`, dan `footer`, serta heading untuk mengelompokkan konten.
- **Aksesibilitas dasar:** gambar memiliki atribut `alt`. Teks alternatif
  dapat dibuat lebih spesifik lagi untuk meningkatkan aksesibilitas.

## Cara Menjalankan

Cara termudah adalah membuka folder proyek di Visual Studio Code dan
menjalankan **Live Server** dari root proyek. Kemudian buka halaman berikut:

- `Page-1/index.html` — landing page GAMIFY.
- `Page-2/src/index.html` — katalog furnitur.

Menjalankan server dari root proyek juga memastikan referensi aset halaman
pertama yang berawalan `/Page-1/` dapat ditemukan.

### Memperbarui CSS Tailwind (opsional)

Jika mengubah kelas Tailwind atau `Page-2/src/input.css`, buka terminal di
folder `Page-2`, lalu jalankan:

```bash
npm install
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

Biarkan proses tersebut berjalan saat mengembangkan halaman katalog. File
`src/output.css` akan diperbarui dan digunakan oleh `src/index.html`.