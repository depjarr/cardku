# cardku — mockup buku diary

Mockup interaktif "card" diri berbentuk buku diary (gaya iPhone) dengan link toko.

## Alamat
- `/` (alamat utama) = **editor** untuk pemilik buku.
- `/#username` (lokal) atau `/username` (di Vercel) = **halaman pengunjung**, view only, tanpa tombol edit.
  Username yang tidak ada akan menampilkan "Buku @username belum ada".

## Cara buka
Klik dua kali `index.html`, atau jalankan server lokal:

    npx http-server . -p 5178 -c-1

- Editor: http://127.0.0.1:5178
- Pengunjung: http://127.0.0.1:5178/#rarashop
- Dari HP (Wi-Fi sama): pakai alamat `http://192.168.x.x:5178` yang muncul di PowerShell.

## Deploy ke Vercel
`vercel.json` sudah mengarahkan `/username` ke `index.html`, jadi `cardku-one.vercel.app/rarashop` langsung jadi halaman pengunjung.

## Isi
- Buku terbuka dua halaman, bisa dibalik (swipe / tombol ‹ ›), tombol Perbesar untuk lihat satu halaman.
- Editor: tambah teks, foto, emoji, stiker 3D, link toko, dan piringan hitam Spotify.
  Geser, cubit untuk zoom, putar dua jari untuk miring, ketuk 2× teks untuk mengetik.
- Font, ukuran, ketebalan, miring, warna, latar teks, efek stiker (Stiker, Puffy, Komik, Shiny).
- Tambah/hapus halaman, ganti latar halaman, 3 tema (Pastel, Kidscore, Apple).
- Tombol Bagikan: salin link pengunjung.

## Catatan penting
- Ini mockup satu file (HTML + CSS + JS). Datanya tersimpan di localStorage browser,
  jadi isi buku belum bisa dilihat dari perangkat lain.
- Pemisahan alamat di mockup baru tampilan. Supaya orang lain benar-benar tidak bisa mengedit,
  versi asli butuh login di alamat editor dan server yang menolak perubahan dari selain pemilik.
- Versi asli juga butuh database per username, penyimpanan foto, dan pemutar Spotify (embed + oEmbed).
