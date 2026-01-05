# LAPORAN PERANCANGAN WEBSITE KIYUTI BOOKSTORE

---

Laporan ini disusun untuk menyelesaikan tugas Pengembangan Web Sisi Klien. Pembuatan website ini dilakukan oleh tiga anggota, diantaranya:

- Ni Putu Tika Wirastari        (240040135)         
- Kadek Yuni Dwiyantini Savitri (240040138) 
- Ni Nyoman Putri Kirana        (240040140) 

## 1. Pendahuluan

### 1.1 Latar Belakang
Kiyuti Bookstore merupakan sebuah website katalog buku yang dikembangkan sebagai media digital untuk menyajikan informasi koleksi buku secara terstruktur dan mudah untuk diakses oleh seluruh kalangan pengguna tanpa batasan ruang dan waktu. Website ini dirancang untuk menjawab permasalahan dalam proses pencarian dan penelusuran informasi buku yang sering kali masih dilakukan secara manual atau tidak terorganisasi dengan baik, sehingga menyulitkan pengguna dalam menemukan buku yang sesuai dengan kebutuhan mereka. Maka dari itu, dari website Kiyuti Bookstore diharapkan dapat meningkatkan kemudahan akses informasi sekaligus memberikan pengalaman pengguna yang lebih efektif, nyaman, dan responsif.

### 1.2 Tujuan Pengembangan Sistem
Tujuan utama dari pengembangan website ini adalah:
- Menyediakan media katalog buku digital yang informatif dan mudah digunakan
- Mempermudah pengguna dalam mencari dan memfilter buku berdasarkan kategori
- Menyajikan informasi buku secara ringkas namun detail
- Meningkatkan kenyamanan pengguna melalui antarmuka yang responsif dan adaptif

---

## 2. Gambaran Umum Sistem

Website Kiyuti Bookstore dikembangkan dengan menggunakan teknologi web standar, yang terdiri dari tiga komponen utama: HTML, CSS, dan JavaScript. Setiap komponen ini berfungsi untuk menyusun struktur, tampilan, dan interaktivitas pada website, memberikan pengalaman pengguna yang optimal.

### 2.1 Struktur File
Berikut adalah struktur folder untuk website Kiyuti Bookstore yang terdiri dari berbagai folder dan file yang digunakan dalam pengembangan website ini:
```text
/Kiyuti-Bookstore-Project-UAS
├── index.html                   → Struktur utama halaman
├── README.md                    → Dokumentasi dan Laporan Sistem
├── /CSS                         → Folder untuk file CSS
│   ├── style.css                → Desain dan tema visual
│   ├── swiper-bundle.min.css    → Stylesheet library Swiper untuk mendukung tampilan slider interaktif.
├── /JS                          → Folder untuk file JS
│   ├── apps.css                 → Logika interaksi dan fitur dinamis
│   ├── swiper-bundle.min.js     → Library JavaScript Swiper untuk mengelola slider buku dan konten beranda.
├── /MEDIA                       → Direktori penyimpanan aset media, seperti gambar sampul buku, dan profile serta kebutuhan visual lainnya
├── /Rancangan.txt               → Berkas perancangan yang memuat semua informasi mengenai kategori buku serta catatan pendukung lainnya.
```
### 3.2 Penjelasan Struktur Komponen 
#### 1. index.html
File index.html merupakan file utama yang memiliki peran penting sebagai struktur dasar dari setiap halaman pada website Kiyuti Bookstore, seperti header, seluruh konten utama website, serta footer. Selain itu, file index.html juga berfungsi untuk menyertakan referensi ke file CSS dan JavaScript yang digunakan untuk mengatur tampilan dan interaktivitas dari website tersebut.

**Fitur yang terdapat pada index.html:**

**- Header dan Navigasi:** Pada bagian ini, terdapat elemen navigasi utama yang dibangun menggunakan **Flexbox** dan **CSS Grid.** Sehingga, tampilan website tetap responsif dan dapat menyesuaikan diri dengan berbagai ukuran perangkat pengguna.

**- Konten Utama (Main Content):** Halaman utama berisi beberapa section penting seperti **Beranda, Daftar Buku, dan Rekomendasi Buku** yang  memiliki fungsi tersendiri untuk menyajikan informasi yang relevan pengguna website.

**- Footer:** Pada bagian footer, terdapat informasi tambahan mengenai **kontak, sosial nedia dan navigasi** sebagai quicklinks yang menghubungkan setiap fitur utama pada website. Footer ini memberikan pengunjung kemudahan untuk mengakses informasi penting dengan cepat yang berkaitan dengan layanan Kiyuti Bookstore.

#### 2. style.css

File style.css yang terdapat pada folder CSS berfungsi untuk mengatur tampilan visual dari website Kiyuti Bookstore, termasuk desain layout, responsivitas tampilan, serta menggunakan :root untuk mengatur warna, font dan typography, font weight.

**A. Desain Layout**

Website ini menggunakan **Flexbox dan CSS Grid** untuk menyusun elemen-elemen pada halaman agar tetap rapi dan responsif. Ini memungkinkan tata letak yang fleksibel dan adaptif, yang dapat menyesuaikan dengan berbagai ukuran layar.

**1) Flexbox:**
Flexbox digunakan untuk mengatur elemen-elemen yang harus berada dalam satu baris (misalnya navigasi) dan menyusun elemen-elemen dalam sebuah kontainer secara dinamis.

**Contoh kode:**
```css
/* Flexbox Layout untuk Navigasi */
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 96px;
}
```
 **2) Grid:**
 CSS Grid digunakan untuk mengatur layout yang lebih kompleks, seperti menata buku-buku dalam kolom atau mengatur elemen konten utama dengan jarak antar elemen

 **Contoh kode:**
 ```css
 /* Grid Layout untuk Konten Buku */
.book-container {
  display: grid;
  gap: 1rem;
}
```
**B. Responsivitas tampilan**

Pada file style.css digunakan untuk mengembangkan code agar tampilan website tetap responsif di berbagai perangkat, baik desktop, tablet, maupun smartphone. Ini dilakukan dengan menggunakan media queries yang memungkinkan pengaturan ukuran elemen berdasarkan lebar layar perangkat menyesuaikan dengan yang digunakan oleh pengguna.

**Contoh kode:**
```css
/* Responsivitas untuk ukuran layar lebih besar (lebih dari 1150px) */
@media screen and (min-width: 1150px) {
  :root {
    --biggest-font-size: 3.5rem;
    --h1-font-size: 2.25rem;
  }
}

/* Responsivitas untuk ukuran layar lebih kecil (maks 768px) */
@media screen and (max-width: 768px) {
  .nav {
    margin: 0 20px;
  }
}
```

