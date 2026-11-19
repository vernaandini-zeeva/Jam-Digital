# Jam Digital — Neon Clock

Jam digital real-time yang dibuat dengan **HTML, CSS, dan JavaScript murni**. Menampilkan waktu komputer dengan format HH:MM:SS dan efek neon glow di atas tema gelap.

> A real-time digital clock with a dark neon-glow theme, built with pure HTML, CSS & JavaScript.

## Fitur

- **Update real-time**: waktu diperbarui setiap detik menggunakan `setInterval`
- **Format HH:MM:SS**: jam, menit, dan detik dengan angka selalu dua digit (`padStart`)
- **Tema neon gelap**: background biru gelap (`#0f172a`) dengan teks biru menyala (`#38bdf8`) dan efek `text-shadow` glow
- **Tampilan besar**: ukuran font 80px dengan letter-spacing lebar, pas untuk layar monitor atau dashboard

## Cara Menjalankan

Buka file `jam.html` langsung di browser (double-click). Jam akan otomatis mengikuti waktu sistem perangkat.

## Cara Kerja Singkat

1. Fungsi `updateClock()` mengambil waktu sekarang lewat objek `Date`
2. Setiap bagian (jam, menit, detik) diformat 2 digit dengan `padStart`
3. Hasilnya ditampilkan di elemen `#clock`, diulang setiap 1000 ms lewat `setInterval`

## Teknologi

- HTML5
- CSS3 (flexbox centering, text-shadow glow)
- JavaScript (`Date`, `setInterval`, `padStart`)

## Struktur File

```
jam.html   # seluruh jam digital (HTML + CSS + JS dalam satu file)
```

## Catatan Pengembangan

- Elemen `<div id="clock">` saat ini ditulis di dalam `<head>`. Browser otomatis memindahkannya ke `<body>` sehingga jam tetap tampil, tetapi sebaiknya dipindahkan ke dalam `<body>` agar HTML valid.
- Ide pengembangan: tampilan tanggal, pilihan format 12/24 jam, tema terang, dan alarm sederhana.
