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
