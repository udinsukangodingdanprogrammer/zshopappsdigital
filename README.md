# ZSHOPAPPS GitHub Pages Package

Paket ini sudah dipisahkan dari satu HTML besar menjadi struktur statis yang siap dipublikasikan melalui GitHub Pages.

## Struktur

- `index.html`: halaman utama GitHub Pages
- `assets/images/`: gambar hasil ekstraksi
- `assets/video/`: video hasil ekstraksi
- `assets/audio/`: enam lagu MP3 hasil ekstraksi
- `assets/files/`: folder file tambahan
- `asset-manifest.json`: daftar aset, ukuran, MIME type, dan SHA-256
- `.nojekyll`: mencegah pemrosesan Jekyll yang tidak diperlukan

## Ringkasan konversi

- HTML asli: 41,378,185 byte
- HTML hasil: 402,481 byte
- Audio terpisah: 6 file
- Data URI diganti: 112 kemunculan
- Data URI unik: 58 file

## Deploy lewat GitHub

1. Buat repository baru.
2. Upload seluruh isi folder ini ke root repository. Jangan upload folder pembungkusnya saja.
3. Buka `Settings`, lalu `Pages`.
4. Pada `Build and deployment`, pilih `Deploy from a branch`.
5. Pilih branch `main` dan folder `/ (root)`, lalu simpan.
6. Tunggu URL GitHub Pages muncul pada halaman yang sama.

Untuk upload melalui browser GitHub, perhatikan batas 25 MiB per file. Jika ada file lebih besar, gunakan Git command line atau GitHub Desktop.

## Format gambar

Semua aset gambar pada folder `assets/images/` telah dikonversi menjadi PNG. Referensi di `index.html` dan `asset-manifest.json` juga sudah diperbarui.

## Update portal digital lifetime

Versi ini menambahkan section terpisah di bawah katalog 20 aplikasi:

- Produk: **ZSHOPAPPS Preflix — Portal Digital**
- Harga jual mulai: **Rp309.000**
- Lisensi: **lifetime / permanen**, mengikuti ruang lingkup yang disepakati dengan owner
- Kanal pembelian produk portal: **Telegram @Seller4899**
- UI pembelian: tabel responsif, jumlah lisensi, total otomatis, ringkasan checkout, dan tombol konfirmasi setelah pembayaran
- Aset baru: `assets/images/portal-lifetime/`

Aset gambar baru sudah menggunakan format PNG dan dipanggil melalui path relatif agar kompatibel dengan GitHub Pages.

Sebelum pembayaran, pembeli harus mengonfirmasi ruang lingkup file, ketentuan lisensi, bantuan instalasi, custom branding, domain/hosting, dan integrasi teknis melalui Telegram owner. Verifikasi pembayaran tetap dilakukan secara manual.


## Update perbaikan katalog gabungan, QRIS, dan aset

- Kelima gambar portal disalin ke `assets/images/` dengan nama sederhana dan path relatif `./assets/images/...`. Folder lama `assets/images/portal-lifetime/` tetap dipertahankan sebagai fallback.
- Katalog sekarang berisi **21 produk**: 20 aplikasi + 1 portal bisnis ZSHOPAPPS Preflix.
- Portal masuk ke keranjang yang sama dengan aplikasi.
- Portal dibatasi **maksimal satu lisensi per nama bisnis**. Nama bisnis wajib diisi saat checkout portal.
- Keranjang yang berisi portal hanya dapat dikonfirmasi melalui Telegram `@Seller4899`.
- QRIS bersifat statis; nominal harus dimasukkan manual sesuai total yang sudah pasti dan bukti pembayaran diverifikasi owner.
- Pembatasan nama bisnis di website statis memakai localStorage perangkat. Validasi global lintas perangkat memerlukan backend/database.
# Update Perbaikan ZSHOPAPPS

Versi ini memperbaiki masalah aset gambar dan menggabungkan produk portal dengan katalog aplikasi.

## Perubahan

- Lima gambar ZSHOPAPPS Preflix tersedia langsung di `assets/images/`.
- Path gambar menggunakan format relatif `./assets/images/...` untuk GitHub Pages.
- Folder lama `assets/images/portal-lifetime/` dipertahankan sebagai fallback.
- Katalog menjadi 21 produk: 20 aplikasi + 1 portal bisnis.
- Portal memakai keranjang yang sama dengan aplikasi.
- Total QRIS dihitung dari seluruh item yang harganya sudah pasti.
- Keranjang yang berisi portal wajib menggunakan Telegram `@Seller4899`.
- Portal maksimal satu lisensi per nama bisnis.
- Nama bisnis wajib diisi sebelum checkout portal.
- FAQ dan cerita alur pembelian ditambahkan.

## Catatan validasi satu bisnis

Pembatasan pada website statis menggunakan `localStorage` perangkat dan batas jumlah pada keranjang. Validasi global lintas perangkat memerlukan backend/database atau pemeriksaan manual oleh owner.

## Cara upload GitHub Pages

Upload seluruh isi ZIP ke root publishing source, termasuk `index.html`, folder `assets`, `.nojekyll`, dan file pendukung. Jangan hanya mengunggah `index.html`.
