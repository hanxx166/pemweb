# Tugas 2 - Pengembangan Aplikasi Web
**Nama  :** Erhan Kurniawan  
**NIM   :** 124140217  
**Kelas :** RA  
**Mata Kuliah:** Pengembangan Aplikasi Web  
**Link GitHub Pages:** https://hanxx166.github.io/pemweb/tugas2/    

---

## 1. Alasan Penggunaan Struktur Semantik

Pada pembuatan website ITERA ini, saya menggunakan elemen-elemen HTML5 semantik dengan alasan sebagai berikut:

- **`<header>`**: Digunakan untuk membungkus bagian kepala halaman yang berisi logo dan identitas situs. Ini memudahkan mesin pencari dan *screen reader* untuk mengidentifikasi bagian pembuka halaman.
- **`<nav>`**: Digunakan khusus untuk menampung menu navigasi utama (Beranda dan Berita). Memisahkan navigasi dari konten utama membuat struktur kode lebih rapi dan aksesibel.
- **`<main>`**: Menandai konten utama dari halaman. Hanya boleh ada satu `<main>` per halaman, sehingga membantu *browser* memahami di mana letak inti informasi.
- **`<article>`**: Digunakan untuk membungkus konten yang berdiri sendiri, seperti artikel berita dan profil institusi. Ini menegaskan bahwa konten tersebut bisa dibaca secara independen.
- **`<section>`**: Digunakan untuk memecah artikel menjadi bagian-bagian tematik, seperti "Sejarah Singkat", "Visi dan Misi", serta "Program Studi". Ini membuat pembaca dan mesin pencari lebih mudah memahami hierarki informasi.
- **`<aside>`**: Digunakan pada halaman berita untuk menampilkan informasi tambahan (sidebar) yang tidak termasuk dalam alur utama artikel, seperti alamat dan kontak ITERA.
- **`<footer>`**: Digunakan untuk menampilkan informasi hak cipta di bagian bawah halaman.
- **Heading Terstruktur (h1-h6)**: Saya menggunakan `<h1>` untuk judul utama halaman, `<h2>` untuk sub-judul bagian, dan `<h3>` untuk sub-bagian di dalam `<aside>`. Ini menjaga hierarki konten agar logis.
- **Tabel**: Saya menggunakan `<table>` pada halaman utama untuk menyajikan data Program Studi ITERA dalam format baris dan kolom agar lebih mudah dibaca.

## 2. Tantangan dan Solusi

Selama proses pengerjaan, terdapat beberapa tantangan teknis yang saya hadapi beserta solusinya:

**Tantangan 1: Nama file gambar mengandung spasi**  
Saat memvalidasi kode di W3C, muncul error `Bad value ./images/Logo ITERA.png for attribute src`. Hal ini disebabkan karena nama file gambar saya mengandung spasi, yang tidak diperbolehkan dalam atribut `src`.  
**Solusi:** Saya mengganti nama file menjadi `LogoITERA.png` (tanpa spasi) dan memperbarui path di dalam kode HTML.

**Tantangan 2: Peringatan (Warning) pada atribut tabel**  
W3C memberikan peringatan bahwa atribut `border` pada elemen `<table>` sudah usang (obsolete) di HTML5.  
**Solusi:** Karena tugas ini mengharuskan penggunaan HTML murni tanpa CSS, saya menghapus atribut `border` dan membiarkan tabel tampil polos. Peringatan ini tidak bersifat fatal (bukan error), sehingga validasi tetap lolos.

**Tantangan 3: Pesan Info pada void elements**  
Validator W3C menampilkan pesan info *"Trailing slash on void elements has no effect..."* pada tag `<meta>` dan `<img>`. Ini terjadi karena saya menambahkan tanda `/` di akhir tag, yang merupakan kebiasaan dari XHTML.  
**Solusi:** Saya menghapus tanda `/` pada tag `<meta charset="UTF-8">`, `<meta name="viewport">`, dan `<img>`. Setelah itu, validasi menjadi bersih tanpa pesan info.

## 3. Hasil Validasi

Berikut adalah bukti hasil validasi kode HTML saya menggunakan W3C Markup Validation Service:

<img width="959" height="509" alt="Screenshot 2026-09-16 213749" src="https://github.com/user-attachments/assets/388957d5-15af-491f-9579-8796f4234d12" />
  
**Gambar 1.** Hasil validasi `index.html` - No errors or warnings.

<img width="959" height="512" alt="Screenshot 2026-09-16 213816" src="https://github.com/user-attachments/assets/4e143201-ff6e-427d-bcfa-c75be9ecd470" />
  
**Gambar 2.** Hasil validasi `berita.html` - No errors or warnings.

## 4. Hosting di GitHub Pages

Website ini telah di-hosting menggunakan GitHub Pages dan dapat diakses melalui tautan berikut:
**[https://hanxx166.github.io/pemweb/tugas2/](https://hanxx166.github.io/pemweb/tugas2/)**

Seluruh tautan navigasi (Beranda dan Berita) serta gambar logo telah dipastikan berfungsi dengan baik.
