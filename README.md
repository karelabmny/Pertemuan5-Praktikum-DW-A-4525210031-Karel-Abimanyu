# Tugas Praktikum Pertemuan 5 - Desain Web

**Nama:** Karel Abimanyu
**NPM:** 4525210031
**Kelas:** A

## Tugas & Bukti Praktikum

Membuat wireframe desktop dan mobile dengan tema Company Profile (Warkop Polim), dalam dua file (`index.html` dan `style.css`), tingkat fidelitas mid-fidelity.

### File

| File | Keterangan |
|------|------------|
| `index.html` | Struktur wireframe (header, navbar, sidebar, hero, tentang, menu unggulan, footer) |
| `css/style.css` | Seluruh CSS (tidak ada CSS inline/internal) |
| `img/` | Folder aset gambar (5 gambar: logo, hero, tentang, dan 2 menu unggulan) |
| `dokumentasi/` | Tangkapan layar tampilan desktop dan mobile |

### Struktur Folder

```
pertemuan-05/
├── index.html
├── README.md
├── css/
│   └── style.css
├── img/
│   ├── logo warkopolim.jpe
│   ├── warkopolim-1.jpe
│   ├── warkopolim-2.jpe
│   ├── kopsu.jpe
│   └── mie.jpe
└── dokumentasi/
    ├── tampilan-desktop.png
    └── tampilan-mobile.png
```

## Yang Dipakai

- **Elemen semantik:** `header`, `nav`, `main`, `aside`, `section`, `article`, dan `footer`.
- **Layout:** CSS Grid untuk layout utama (sidebar + konten), hero, tentang, dan card menu; Flexbox untuk header, navbar, sidebar, dan footer.
- **Gambar:** 5 gambar di folder `img/`, dipasang dengan `<img>` dan `object-fit: cover` agar proporsi terjaga.
- **Media query:** `@media (max-width: 900px)` untuk tablet dan `@media (max-width: 640px)` untuk smartphone.

## Screenshot

### Tampilan Desktop

![Tampilan desktop company profile Warkop Polim] <img width="670" height="932" alt="ss-desktop" src="https://github.com/user-attachments/assets/7bad656a-5ce9-49d9-9b89-750d24c0ad55" />

### Tampilan Mobile

![Tampilan mobile company profile Warkop Polim] <img width="800" height="5922" alt="ss-mobile" src="https://github.com/user-attachments/assets/6db5ba93-8f8b-42a6-ac6b-8effd193a9dc" />

## Ringkasan Solusi

Pada tugas ini saya membuat wireframe mid-fidelity bertema Company Profile dengan studi kasus Warkop Polim, dalam dua file terpisah yaitu `index.html` untuk struktur dan `style.css` untuk tampilan. Struktur halaman mengikuti anatomi standar, yaitu header, navbar, sidebar (kategori menu dan jam buka), konten utama (hero, tentang, dan menu unggulan), serta footer yang berisi kontak dan media sosial, dengan elemen semantik agar susunannya jelas. Gambar yang dipakai sudah dipasang pada tiap area (logo, hero, tentang, dan menu) agar proporsi tiap bagian terlihat nyata. Masalah yang muncul pertama adalah ukuran foto yang tidak seragam, sehingga gambar terlihat gepeng atau tidak sejajar. Solusinya, semua foto konten diberi rasio 4:3 dengan `object-fit: cover`. Masalah kedua adalah sidebar, card menu, dan navbar yang terlalu sempit jika tetap berjajar di layar kecil. Solusinya, saya menambahkan dua media query: pada lebar maksimal 900px hero menjadi satu kolom dan lebar sidebar diperkecil, lalu pada lebar maksimal 640px semua elemen disusun satu kolom, navbar menjadi menu vertikal, dan sidebar dipindah ke bawah konten utama. Hasilnya diuji pada ukuran desktop dan mobile tanpa scroll horizontal, sehingga kerangka halaman siap dilanjutkan ke tahap mockup visual pada pertemuan berikutnya.
