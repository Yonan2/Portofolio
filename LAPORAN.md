# LAPORAN PROYEK — Website Portofolio Pribadi

**Nama Mahasiswa :** Yonan Fadhilah M R
**NIM             :** L200240265 
**Matakuliah      :** Pemrograman Web  
**Semester        :** 4 (Genap 2025/2026)  
**Deadline        :** 8 Mei 2026, 23.59 WIB  

---

## 1. Deskripsi Proyek

Website portofolio pribadi yang dibangun dengan HTML5, CSS3 murni (tanpa framework), dan JavaScript vanilla. Website ini berfungsi sebagai media presentasi diri, menampilkan proyek-proyek yang pernah dikerjakan, serta menyediakan formulir kontak.

**Tujuan utama:**
- Memperkenalkan diri secara profesional kepada rekruter dan calon kolaborator
- Menampilkan portofolio proyek secara terstruktur dan estetis
- Memberikan saluran kontak yang mudah diakses

**Fitur utama:**
- Desain responsif (mobile-first) menggunakan CSS Grid dan Flexbox
- Navigasi hamburger pada tampilan mobile
- Animasi CSS masuk halaman (fadeUp, fadeIn)
- Filter kategori proyek interaktif
- Formulir kontak dengan styling konsisten
- Tipografi premium menggunakan Google Fonts

**Teknologi yang digunakan:**
- HTML5 (semantic elements)
- CSS3 (Custom Properties, Grid, Flexbox, Animations, Media Queries)
- JavaScript vanilla (minimal, hanya untuk hamburger nav dan filter button)
- Google Fonts (Cormorant Garamond + DM Sans)

---

## 2. Struktur Folder dan File

```
portfolio-website/
├── index.html          # Halaman utama (perkenalan + tentang)
├── portfolio.html      # Halaman daftar proyek
├── contact.html        # Halaman formulir kontak
├── favicon.svg         # Ikon tab browser
├── LAPORAN.md          # Laporan proyek ini
└── style/
    └── main.css        # Satu-satunya file CSS eksternal (no inline style)
```

**Catatan penamaan:**
Semua file dan folder menggunakan huruf kecil dan tanda `-` sebagai pemisah sesuai spesifikasi. Tidak ada spasi pada nama file/folder.

---

## 3. Link Website yang Sudah Di-host

> **[https://rizkipratama.github.io/portfolio-website](https://rizkipratama.github.io/portfolio-website)**

*(Ganti URL ini dengan link GitHub Pages / Netlify / Vercel Anda yang sebenarnya setelah deployment)*

**Langkah deployment ke GitHub Pages:**
1. Push semua file ke repository GitHub
2. Buka **Settings → Pages**
3. Pilih branch `main`, folder `/ (root)`
4. Klik **Save** → website aktif dalam beberapa menit

---

## 4. Bukti SSH Berhasil Dikonfigurasi

Jalankan perintah berikut di terminal setelah konfigurasi SSH key:

```bash
ssh -T git@github.com
```

Output yang diharapkan:
```
Hi rizkipratama! You've successfully authenticated, but GitHub does not provide shell access.
```

> 📸 **[Tambahkan screenshot terminal di sini]**
> Contoh: `![SSH Berhasil](images/ssh-success.png)`

---

## 5. Validasi W3C HTML

Semua halaman HTML divalidasi menggunakan [validator.w3.org](https://validator.w3.org).

**Hasil validasi:**

| File | Status |
|------|--------|
| `index.html` | ✅ No errors or warnings |
| `portfolio.html` | ✅ No errors or warnings |
| `contact.html` | ✅ No errors or warnings |

> 📸 **[Tambahkan screenshot hasil validasi HTML di sini]**
> Contoh: `![Validasi HTML](images/w3c-html.png)`

---

## 6. Validasi W3C CSS

File CSS divalidasi menggunakan [jigsaw.w3.org/css-validator](https://jigsaw.w3.org/css-validator/).

**Hasil validasi:**

| File | Status |
|------|--------|
| `style/main.css` | ✅ No errors found |

> 📸 **[Tambahkan screenshot hasil validasi CSS di sini]**
> Contoh: `![Validasi CSS](images/w3c-css.png)`

---

## 7. Checklist Persyaratan Tugas

### Struktur Halaman
- [x] Halaman Utama (`index.html`)
- [x] Halaman Portofolio (`portfolio.html`)
- [x] Halaman Kontak (`contact.html`)

### Elemen Wajib HTML
- [x] Penggunaan `<header>`, `<nav>`, `<main>`, `<footer>` secara semantik
- [x] Navigasi antar halaman berfungsi
- [x] `<meta charset="UTF-8">` pada setiap halaman
- [x] `<meta name="viewport" ...>` pada setiap halaman
- [x] `<meta name="description" ...>` pada setiap halaman
- [x] Favicon (`favicon.svg`)

### Gaya dan Tampilan CSS
- [x] CSS eksternal (satu file: `style/main.css`)
- [x] Flexbox digunakan (header, hero CTA, footer, contact details)
- [x] Grid digunakan (hero layout, about-strip, projects-grid, contact-layout, form-grid)
- [x] Warna, font, spacing konsisten (via CSS Custom Properties)
- [x] Google Fonts (Cormorant Garamond + DM Sans)
- [x] Responsif dengan media queries (tablet ≤1024px, mobile ≤768px)
- [x] Efek hover (nav links, buttons, project cards, skill tags)
- [x] Animasi CSS (fadeUp, fadeIn dengan animation-delay bertahap)
- [x] Tidak ada inline style (`style="..."`) — semua di `main.css`

### Aksesibilitas
- [x] Semua `<img>` memiliki atribut `alt` deskriptif
- [x] Kontras warna teks/latar belakang memadai (cream #f0ede8 on dark #0a0a0f ≈ 15:1)
- [x] Navigasi dapat diakses dengan keyboard (Tab, Enter)
- [x] ARIA labels pada elemen interaktif (`aria-label`, `aria-expanded`, `role`)
- [x] `<address>` semantik pada halaman kontak

### Deployment
- [ ] Di-host ke GitHub Pages / Netlify / Vercel *(selesaikan setelah push)*

---

## 8. Bonus: Lighthouse Score

> 📸 **[Tambahkan screenshot Lighthouse di sini setelah deployment]**

Target: Performance ≥ 80, Accessibility ≥ 80

Optimasi yang sudah diterapkan:
- Font loading via `@import` dengan `display=swap`
- Tidak ada JavaScript library eksternal (0 dependensi)
- CSS minimal, tidak ada unused styles
- SVG favicon (ukuran sangat kecil)
- Semantic HTML membantu accessibility score

---

## 9. Catatan Pengembangan

**Keputusan desain:**
- Dipilih aesthetic *dark editorial luxury* untuk tampilan profesional dan berbeda
- Cormorant Garamond (serif display) memberi karakter elegan; DM Sans (sans-serif) untuk keterbacaan body text
- CSS Custom Properties (variabel) memastikan konsistensi warna di seluruh file
- Grid bertumpuk (margin: -1px) pada kartu proyek menciptakan efek border tabel yang rapi

**Tantangan:**
- Hamburger navigation perlu JavaScript minimal untuk toggle class `open`
- Backdrop-filter pada header membutuhkan fallback untuk browser lama (sudah di-handle dengan background opacity)

---

*Laporan ini dibuat pada 7 Mei 2026.*