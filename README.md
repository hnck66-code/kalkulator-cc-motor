# Kalkulator CC Motor — PWA

Aplikasi web untuk menghitung kapasitas geometris mesin satu silinder berdasarkan bore dan stroke.

## Isi proyek

- `index.html` — antarmuka, CSS, dan logika kalkulator.
- `manifest.json` — metadata instalasi PWA.
- `service-worker.js` — cache agar aplikasi dapat dibuka offline setelah kunjungan pertama yang berhasil.
- `icons/` — ikon aplikasi PNG ukuran 192×192 dan 512×512, termasuk ikon maskable.

## Rumus

`CC = (π / 4) × bore² × stroke / 1000`

Bore dan stroke dimasukkan dalam milimeter. Kalkulator menerima desimal dengan titik atau koma.

## Publikasikan lewat GitHub Pages

1. Masuk ke GitHub dan buat repository baru, misalnya `kalkulator-cc-motor`.
2. Unggah **isi folder proyek ini** ke root repository. Pastikan `index.html`, `manifest.json`, dan `service-worker.js` terlihat langsung di root, bukan di dalam folder tambahan.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/(root)`, lalu tekan **Save**.
6. Tunggu proses deploy selesai. Alamat umumnya `https://USERNAME.github.io/NAMA-REPOSITORY/`.
7. Buka alamat HTTPS tersebut di Chrome Android dan tunggu halaman selesai dimuat sekali saat online.

## Pasang di Android

1. Buka alamat GitHub Pages di Chrome.
2. Tekan menu titik tiga (⋮).
3. Pilih **Install app / Instal aplikasi** jika tersedia. Jika tidak, pilih **Add to Home screen / Tambahkan ke layar utama**.
4. Konfirmasi. Ikon **Hitung CC** akan muncul di layar utama atau daftar aplikasi.

## Catatan

- PWA perlu diakses melalui HTTPS atau localhost agar service worker aktif; file HTML yang dibuka langsung dari penyimpanan tidak menyediakan semua fitur PWA.
- Setelah kunjungan pertama berhasil, halaman dan perhitungan dapat digunakan offline. Perubahan versi aplikasi dapat memerlukan pemuatan ulang.
- GitHub Pages bersifat publik: siapa pun yang memiliki alamat repository/website dapat membukanya.
