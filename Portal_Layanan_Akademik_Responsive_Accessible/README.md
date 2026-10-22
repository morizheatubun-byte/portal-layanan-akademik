# Portal Layanan Akademik

Proyek web client statis untuk tugas **Responsive & Accessible Web Client**.

## Struktur
- `index.html` — struktur halaman semantik dan formulir.
- `css/styles.css` — desain mobile-first, layout Grid/Flexbox, focus indicator, dan breakpoint.
- `evidence/` — tempat menyimpan screenshot hasil pengujian DevTools.

## Menjalankan
1. Ekstrak folder proyek.
2. Buka `index.html` di browser, atau gunakan ekstensi Live Server di VS Code.
3. Halaman tidak memerlukan instalasi package maupun JavaScript.

## Fitur
- Landmark semantik: `header`, `nav`, `main`, `section`, `article`, `form`, `footer`.
- Tiga kartu layanan akademik.
- Form nama, NIM, email, jenis layanan, dan keperluan dengan validasi HTML.
- Skip link, label terasosiasi, focus indicator yang terlihat, dan tata letak responsif.
- Form merupakan demo antarmuka dan belum menyimpan data ke server.

## Checklist pengujian DevTools (isi setelah pengujian nyata)
Lakukan pengujian di browser Anda dan simpan screenshot ke folder `evidence/`.

| Pengujian | Cara | Hasil yang harus diperiksa |
|---|---|---|
| Responsive 360 px | DevTools → Toggle Device Toolbar → set width 360 | Tidak ada scroll horizontal; teks dan form tetap terbaca |
| Responsive 768 px | Set width 768 | Kartu dan form menyesuaikan ruang |
| Responsive 1280 px | Set width 1280 | Tiga kartu sejajar dan konten tidak terlalu melebar |
| Elements/Inspector | Periksa DOM dan computed CSS | Landmark, heading, label, dan breakpoint sesuai |
| Keyboard | Reload lalu tekan Tab | Skip link dan fokus kontrol terlihat |
| Validasi form | Kirim saat kosong; masukkan email tidak valid | Browser menolak input wajib/email invalid |
| Network | Buka Network, reload halaman | `index.html` dan `css/styles.css` berhasil dimuat; tidak ada resource gagal |
| Accessibility | Periksa accessibility tree/inspector yang tersedia | Nama kontrol berasal dari label; heading berurutan |

**Penting:** checklist ini adalah panduan pengujian, bukan klaim bahwa screenshot atau pengujian sudah dilakukan. Ambil screenshot aktual dan letakkan di `evidence/`.
