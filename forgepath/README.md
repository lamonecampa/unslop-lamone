# ForgePath — Jalur Belajar Laravel

Portal belajar statis berbahasa Indonesia untuk pemula total. Jalur lengkap: pengenalan web → HTML → CSS → logika pemrograman → PHP → MySQL → Laravel.

## Fitur
- Jalur belajar tiga tahap dengan ringkasan tujuan dan estimasi belajar.
- Daftar bab per tahap, bisa dibuka dan ditandai selesai.
- Progres belajar tersimpan di `localStorage` browser.
- Pencarian materi dengan tombol Cari atau `Ctrl/Cmd + K`.
- Responsif untuk desktop dan perangkat seluler.
- Tautan menuju modul referensi NeonWebId dan dokumentasi Laravel.

## Menjalankan lokal
Buka `index.html` langsung di browser, atau jalankan server statis:
```bash
python -m http.server 8000
```
Kemudian buka `http://localhost:8000`.

## Deploy GitHub Pages
1. Buka Settings → Pages.
2. Pada Build and deployment pilih Deploy from a branch.
3. Pilih branch `main` dan folder `/ (root)`, lalu Save.
4. Tunggu GitHub Pages menerbitkan situs.

Portal ini hanya frontend statis. Tidak ada backend, akun pengguna, sinkronisasi progres lintas perangkat, atau database.

## Sumber materi
- PHP: https://neon.web.id/modul/belajar-php-untuk-pemula/
- MySQL: https://neon.web.id/modul/belajar-mysql-untuk-pemula/
- Laravel: https://neon.web.id/modul/belajar-laravel-untuk-pemula/
- Dokumentasi Laravel: https://laravel.com/docs

## Arah desain
Antarmuka mengikuti prinsip desain yang terdokumentasi pada [Unslop](https://github.com/lamonecampa/unslop-lamone): permukaan netral, satu aksen utama, jarak konsisten, hierarki tipografi, ikon secukupnya, dan tanpa gradien/glow dekoratif.

Unslop dibuat oleh Damir Sokolovsky dan berlisensi CC BY 4.0. ForgePath adalah implementasi desain terpisah, bukan bagian resmi dari proyek Unslop.

## Jalur pemula dari nol
Buka `start.html` untuk materi pengantar yang mencakup cara kerja website, HTML, CSS, logika pemrograman, PHP, MySQL, dan Laravel. Halaman ini memiliki contoh HTML yang dapat dicoba langsung, latihan per tahap, dan checklist progres lokal.


## ForgePath practice suite
- `php-lab.html`: editor latihan dan instruksi menjalankan PHP melalui interpreter/server lokal. Tidak mengklaim menjalankan PHP di browser.
- `sql-lab.html`: SQL interaktif memakai SQLite WebAssembly dengan database contoh sementara di memori browser. Sintaks SQLite tidak identik sepenuhnya dengan MySQL.
- `quiz.html`: 12 pertanyaan evaluasi dengan skor dan pembahasan.
- `projects.html`: empat proyek bertahap dari profil pribadi sampai aplikasi Laravel, checklist, dan rubrik mandiri.

## Batasan teknis
Semua halaman tetap statis. Progres tersimpan di localStorage pada browser/perangkat masing-masing, bukan tersinkronisasi lintas perangkat. SQL Lab memerlukan koneksi internet untuk memuat library sql.js dari CDN. PHP Lab memerlukan instalasi PHP lokal atau server PHP sungguhan. Jangan masukkan data rahasia ke latihan.
