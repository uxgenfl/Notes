# Nexus Notes

Aplikasi catatan statis: satu file `index.html`, tanpa build dan tanpa dependensi eksternal.
Font Geist sudah tertanam. Catatan tersimpan di browser pemakai (localStorage).
Bisa dipasang di layar utama (PWA) dan tetap terbuka saat offline.

## Isi

- `index.html`: aplikasi
- `manifest.json`, `sw.js`: PWA dan cache offline
- `icon.svg`, `favicon-32.png`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png`: ikon sesuai Nexus Brand Kit (plat Ink, simbol N dengan Seam, bar aksen Umber)
- `.nojekyll`: supaya GitHub Pages menyajikan file apa adanya

## Cara upload ke GitHub Pages

1. Buat repository baru di GitHub (misalnya `nexus-notes`).
2. Upload semua isi zip ini ke root repository, termasuk `.nojekyll`.
3. Buka **Settings → Pages**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
4. Tunggu 1-2 menit. Alamatnya: `https://USERNAME.github.io/nexus-notes/`

## Catatan

- Setelah mengganti `index.html`, naikkan versi cache di `sw.js` (`nexus-notes-v2` menjadi `v3`) agar pemakai mendapat versi terbaru.
- Data tersimpan per browser dan per alamat situs. Gunakan **Pengaturan > Kontrol data > Ekspor** untuk cadangan.
- Font Geist: lisensi SIL Open Font License 1.1.
