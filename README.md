# cardku — mockup buku diary

Mockup interaktif "card" diri berbentuk buku diary (gaya iPhone) dengan link toko.

## Cara buka
Klik dua kali `index.html`, atau jalankan server lokal:

    npx http-server . -p 5178

lalu buka http://localhost:5178

## Isi
- Buku terbuka dua halaman, bisa dibalik (swipe / tombol ‹ ›), tombol Perbesar untuk lihat satu halaman.
- Mode Edit: tambah teks, foto, emoji, stiker 3D, link toko, dan piringan hitam Spotify.
  Geser, cubit untuk zoom, putar dua jari untuk miring, ketuk 2× teks untuk mengetik.
- Font, ukuran, ketebalan, miring, warna, latar teks, efek stiker (Stiker, Puffy, Komik, Shiny).
- Tambah/hapus halaman, ganti latar halaman, 3 tema (Pastel, Kidscore, Apple).
- Mode Pengunjung: view only, link toko bisa diklik.

## Catatan
- Ini mockup satu file (HTML + CSS + JS), datanya tersimpan di localStorage browser.
- Versi asli nanti butuh login, database per username (halaman `/username`),
  penyimpanan foto, dan pemutar Spotify (embed + oEmbed untuk sampul album).
