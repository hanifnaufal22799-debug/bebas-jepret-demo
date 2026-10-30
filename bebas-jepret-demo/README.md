# Bebas Jepret — Interactive Demo

Website demo statis untuk presentasi Bebas Jepret. Dibuat dengan HTML, CSS, dan JavaScript murni agar bisa di-host gratis menggunakan GitHub Pages.

## Isi project

```text
bebas-jepret-demo/
├── index.html
├── style.css
├── script.js
├── README.md
├── .nojekyll
└── assets/
    ├── logo.png                 # placeholder BJ, bukan logo resmi
    ├── demo-data.js             # metadata 10 template + koordinat slot
    ├── templates/               # 10 preview template dari aset software asli
    └── photos/                  # foto ilustrasi dummy, bukan foto pelanggan
```

## Fitur demo

- Halaman utama dengan pilihan Customer Demo dan Admin Dashboard.
- Pilih foto dummy, pilih template, pilih slot, geser dan zoom foto.
- Simpan beberapa cetakan, hapus cetakan, tambah template, dan export semua (maksimal 12 cetakan).
- Export menampilkan QR ilustrasi (bukan QR yang dapat dipakai membuka Drive).
- Dashboard admin menampilkan sesi export dari browser yang sama melalui `localStorage`.
- Menjelaskan simulasi folder Google Drive per customer dan penghapusan otomatis 24 jam / pemeriksaan 5 menit.
- Seluruh fungsi cloud, pembayaran, database, dan penghapusan file sungguhan sengaja tidak diaktifkan.

## Menjalankan di komputer

Buka `index.html` langsung di browser modern. Untuk pengalaman yang lebih konsisten, jalankan server statis lokal (opsional), misalnya ekstensi Live Server di VS Code. Tidak perlu Python, Flask, Node, database, API key, atau server backend.

## Upload ke GitHub Pages (gratis)

1. Ekstrak ZIP ini di komputer. Pastikan file `index.html` berada di folder utama `bebas-jepret-demo`, bukan di dalam folder bertingkat lain.
2. Masuk ke https://github.com dan login.
3. Klik **New repository**.
4. Isi nama repository, misalnya `bebas-jepret-demo`.
5. Pilih **Public**, lalu klik **Create repository**.
6. Di halaman repository, klik **Add file → Upload files**.
7. Buka folder hasil ekstrak di komputer, lalu seret semua isi folder (termasuk `index.html`, `style.css`, `script.js`, `README.md`, `.nojekyll`, dan folder `assets`) ke area upload GitHub. Jangan mengunggah ZIP sebagai satu file.
8. Tunggu upload selesai. Isi pesan commit, misalnya `Upload Bebas Jepret demo`, lalu klik **Commit changes**.
9. Buka tab **Settings** repository.
10. Pilih **Pages** di menu sebelah kiri.
11. Pada bagian **Build and deployment**, pilih **Deploy from a branch**.
12. Pada **Branch**, pilih `main` dan folder `/ (root)`, lalu klik **Save**.
13. Tunggu beberapa menit. Refresh halaman **Settings → Pages** sampai alamat website muncul.
14. Link biasanya berbentuk `https://USERNAME.github.io/bebas-jepret-demo/` (ganti `USERNAME` dengan username GitHub kamu).

## Mengganti placeholder logo

Logo resmi belum tersedia pada ZIP software yang diperiksa. File `assets/logo.png` adalah placeholder berinisial BJ, bukan logo resmi. Header sudah menggunakan file ini. Setelah memiliki logo resmi, cukup ganti `assets/logo.png` dengan file logo Bebas Jepret milikmu (pertahankan nama file tersebut).

## Catatan privasi & batasan demo

- Project ini **tidak menyertakan** database SQLite, `.env`, credentials, folder `.venv`, foto customer, file hasil export, atau QR dari sesi asli.
- Hanya sepuluh gambar template preview yang dipilih dari folder template software asli, dikompres ke WebP, serta koordinat slot template yang dibaca dari metadata database. Database asli tidak disalin.
- Data sesi demo tersimpan di `localStorage` browser. Karena GitHub Pages hanya hosting statis, data dari browser/perangkat berbeda tidak akan tersinkron.
- QR pada halaman export hanya pola ilustrasi dan tidak dapat digunakan untuk mengunduh file.
- Semua sesi, status upload, dan jadwal penghapusan adalah data simulasi. Tidak ada koneksi Google Drive dan tidak ada file yang dihapus.
