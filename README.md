# Purplify - Mid Project Web Design

Website pemutar musik bertema ungu (HTML + CSS + Bootstrap 5).
Semua file (Bootstrap, ikon, font) sudah lokal, jadi bisa dibuka **tanpa internet**.

## Cara menjalankan
Buka `index.html` di browser (klik dua kali). Tidak perlu server.

## Halaman
| File | Isi |
|---|---|
| `index.html` | Home: hero carousel, Top 10 lagu, suasana, fitur, form newsletter |
| `playlist.html` | Playlist Top 10, tab playlist suasana, galeri + modal |
| `search.html` | Form pencarian + filter genre (CSS saja) |
| `login.html` | Login & Register (tab) |

## PENTING: ganti MP3 placeholder dengan lagu asli
Folder `audio/` saat ini berisi **nada beep 8 detik** sebagai placeholder supaya player bisa dites.
Timpa dengan file MP3 lagu asli, **dengan nama file yang sama persis**:

```
audio/01-komang.mp3
audio/02-hati-hati-di-jalan.mp3
audio/03-sial.mp3
audio/04-nina.mp3
audio/05-bertaut.mp3
audio/06-lathi.mp3
audio/07-terlalu-lama-sendiri.mp3
audio/08-melukis-senja.mp3
audio/09-sampai-jadi-debu.mp3
audio/10-kota-ini-tak-sama-tanpamu.mp3
```
Jika ingin mengganti lagu/nama file, ubah atribut `src="audio/..."` di `index.html`, `playlist.html`, dan `search.html`.

## Checklist ketentuan tugas
- 4 halaman, Navbar, Hero (Carousel), 5 section di Home, 10+ card, 40+ gambar, Gallery, 4 form, Footer
- Komponen Bootstrap: Navbar, Carousel, Card, Tabs/Pills, Modal, Badge, Input group, Form floating, Grid
- Custom CSS: `css/style.css`
- Responsive: Bootstrap grid + media query
- JavaScript: hanya bawaan Bootstrap (`js/bootstrap.bundle.min.js`), tidak ada JS buatan sendiri

## Catatan
- Pemutar memakai elemen HTML5 `<audio controls>`, jadi lagu bisa diputar tanpa JavaScript. Konsekuensinya, beberapa lagu bisa berbunyi bersamaan jika tidak dijeda manual.
- Kotak pencarian pada halaman Search hanya tampilan (tanpa JS tidak bisa menyaring teks). Filter genre berfungsi memakai CSS `:has()`.
- Form belum terhubung ke server (`action="#"`) karena proyek ini website statis.
