# KIYUTI BOOKSTORE WEBSITE

---

Laporan ini disusun untuk menyelesaikan tugas Pengembangan Web Sisi Klien. Pembuatan website ini dilakukan oleh tiga anggota, diantaranya:

1. Ni Putu Tika Wirastari        (240040135) 
   - Github: @Putu-Kartika
   - Peran: Membuat kategori buku, rekomendasi, dan buku terbaru hingga dapat melakukan pembelian.
2. Kadek Yuni Dwiyantini Savitri (240040138) 
   - Github: Yuni18-git
   - Peran: Membuat navigasi, Membuat fitur tema gelap dan terang, Memperbaiki responsif website.
3. Ni Nyoman Putri Kirana        (240040140) 
   - Github: @Kirana0219
   - Peran: Membuat fitur testimoni, Kontak, Footer serta membuat laporan melalui md



## 1. Deskripsi Sistem
Kiyuti Bookstore merupakan sebuah website katalog buku yang dikembangkan sebagai media digital untuk menyajikan informasi koleksi buku secara terstruktur dan mudah untuk diakses oleh seluruh kalangan pengguna tanpa batasan ruang dan waktu. Website ini dirancang untuk menjawab permasalahan dalam proses pencarian dan penelusuran informasi buku yang sering kali masih dilakukan secara manual atau tidak terorganisasi dengan baik, sehingga menyulitkan pengguna dalam menemukan buku yang sesuai dengan kebutuhan mereka. Maka dari itu, dari website Kiyuti Bookstore diharapkan dapat meningkatkan kemudahan akses informasi sekaligus memberikan pengalaman pengguna yang lebih efektif, nyaman, dan responsif.

### Tujuan Pengembangan Sistem
Tujuan utama dari pengembangan website ini adalah:
- Menyediakan media katalog buku digital yang informatif dan mudah digunakan
- Mempermudah pengguna dalam mencari dan memfilter buku berdasarkan kategori
- Menyajikan informasi buku secara ringkas namun detail
- Meningkatkan kenyamanan pengguna melalui antarmuka yang responsif dan adaptif

---

## 2. Gambaran Umum Sistem

Website Kiyuti Bookstore dikembangkan dengan menggunakan teknologi web standar, yang terdiri dari tiga komponen utama: HTML, CSS, dan JavaScript. Setiap komponen ini berfungsi untuk menyusun struktur, tampilan, dan interaktivitas pada website, memberikan pengalaman pengguna yang optimal.

### Struktur File
Berikut adalah struktur folder untuk website Kiyuti Bookstore yang terdiri dari berbagai folder dan file yang digunakan dalam pengembangan website ini:
```text
/Kiyuti-Bookstore-Project
├── index.html                   → Mengatur struktur dasar setiap website
├── README.md                    → Dokumentasi dan Laporan Sistem
├── /CSS                         → Folder untuk file CSS
│   ├── style.css                → Desain dan tema visual utama
│   ├── swiper-bundle.min.css    → Stylesheet library Swiper untuk mendukung tampilan slider interaktif
├── /JS                          → Folder untuk file JavaScript
│   ├── apps.js                  → Logika interaksi dan fitur dinamis
│   ├── swiper-bundle.min.js     → Library JavaScript Swiper untuk mengelola slider buku dan konten beranda
├── /MEDIA                       → Direktori penyimpanan aset media, seperti gambar sampul buku, dan profile
├── /Rancangan.txt               → Berkas perancangan yang memuat semua informasi mengenai kategori buku
```

### Teknologi yang digunakan

Adapun teknologi yang digunakan untuk pengembangan Website ini, diantaranya sebagai berikut:

**1. HTML (HyperText Markup Language) :**
HTML merupakan file utama yang memiliki peran penting sebagai struktur dasar dari setiap halaman pada website Kiyuti Bookstore, seperti header, seluruh konten utama website, serta footer. Selain itu, file index.html juga berfungsi untuk menyertakan referensi ke file CSS dan JavaScript yang digunakan untuk mengatur tampilan dan interaktivitas dari website tersebut.

**2. CSS (Cascading Style Sheets) :**
CSS berfungsi untuk mengatur tampilan visual dari website Kiyuti Bookstore, termasuk desain layout, responsivitas tampilan, serta menggunakan :root untuk mengatur warna, font dan typography, font weight.

**3. javaScript :**
JavaScript berfungsi untuk memberikan interaktivitas pada halaman wen, seperti pengaturan tema gelap/terang, pencarian, dan filter kategori. JavaScript juga memungkinkan perubahan konten halaman secara dinamis tanpa perlu memuat ulang halaman.

**4. Swiper :**
Swiper adalah library JavaScript untuk membuat slider gambar atau konten di halaman web. Library ini memungkinkan pengguna untuk menggulirkan konten secara interaktif, baik dengan sentuhan atau klik, dan memiliki berbagai efek transisi yang menarik.

**5. Remix Icons :**
Remix Icons adalah koleksi ikon berbasis SVG yang digunakan untuk memperindah tampilan web. Ikon ini menggantikan teks untuk menunjukkan fungsi tertentu, seperti ikon pencarian atau profil, dan dapat disesuaikan ukurannya tanpa kehilangan kualitas visual.

## Fitur Utama Website
**1. Navigasi Responsive :** Navigasi utama pada website menggunakan Flexbox untuk memastikan tampilan menu yang fleksibel dan responsif di berbagai perangkat. Pengguna dapat dengan mudah menavigasi ke berbagai bagian seperti Beranda, Daftar Buku, Rekomendasi, dan Testimoni.

**2. Filter Kategori Buku :** Pengguna dapat memfilter buku berdasarkan kategori tertentu melalui fitur dropdown, seperti Romantis, Fantasi, Horor, dll. Fitur ini memungkinkan pengguna untuk melihat buku dalam kategori yang mereka minati, tanpa harus mencari satu per satu.

**3. Infinite Testimonial :** Website ini menampilkan testimonial pelanggan yang tak terbatas (infinite scrolling). Testimoni ini digulirkan secara otomatis atau dengan tombol navigasi sehingga pengguna dapat terus melihat feedback dari pelanggan yang puas dengan layanan Kiyuti Bookstore tanpa perlu memuat halaman baru.

**4. Modal Buku :** Ketika pengguna mengklik buku dalam katalog, modal akan muncul yang menampilkan informasi lebih lanjut tentang buku tersebut, seperti judul, penulis, deskripsi, harga, bahkan memasukan produk buku kedalam keranjang atau membelinya tanpa harus berpindah halaman.

**5. Tema Gelap dan Terang :** Pengguna dapat mengubah tema website antara tema gelap dan terang. Preferensi tema ini disimpan menggunakan localStorage untuk menjaga konsistensi tampilan setiap kali pengguna kembali ke website.

**6. Home Swiper :** Home Swiper digunakan untuk menampilkan gambar-gambar buku rekomendasi di beranda website. Gambar-gambar ini akan digulirkan secara horizontal dalam bentuk carousel, memberikan pengalaman yang dinamis dan interaktif bagi pengguna. Fitur ini menarik perhatian pengguna dengan cara menampilkan koleksi buku yang diunggulkan atau buku rekomendasi dengan cara yang interaktif dan responsif.

**7. Fitur Alert :** Fitur Alert digunakan untuk menampilkan pesan pemberitahuan atau notifikasi kepada pengguna di website Kiyuti Bookstore. Alert ini bisa digunakan untuk berbagai tujuan, seperti memberi tahu pengguna tentang informasi terbaru, kesalahan, keberhasilan aksi tertentu, atau pembaruan sistem. Fitur ini memberikan umpan balik visual yang penting untuk memastikan bahwa pengguna memahami status atau hasil dari interaksi mereka dengan website.

**8. Slider Buku :** Fitur Slider Buku di website Kiyuti Bookstore digunakan untuk menampilkan buku-buku rekomendasi, buku terbaru, maupun kategori buku lainnya secara dinamis. Gambar buku akan digulirkan secara horizontal dalam format carousel, memberikan pengalaman interaktif dan menarik bagi pengguna yang sedang mencari buku.

## Cara Menajalankan Website
Untuk mengakses dan menjalankan proyek Kiyuti Bookstore, Anda dapat mengikuti langkah-langkah berikut:

### 1. Cloning Github
- Buka terminal/command prompt pada komputer Anda.
- Gunakan perintah berikut untuk mengkloning repositori proyek dari GitHub:
```text
https://github.com/Kirana0219/Kiyuti-Bookstore-Project-UAS.git
```
- Kemudian dapat mengaksesnya melalui live-server atau membuka index.html pada browser seperti Google Chrome, Mozilla Firefox, atau browser lain yang Anda sukai.
### 2. Mengakses melaluui Github Pages
- Membuka browser seperti Google Chrome, Mozilla Firefox, atau browser lain yang Anda sukai.
- Klik atau salin link GitHub Pages berikut:
```teks
https://kirana0219.github.io/Kiyuti-Bookstore-Project-UAS/
```
- Setelah mengklik tautan atau menempelkannya di bilah alamat browser, tekan Enter untuk membuka halaman website.
- Sekarang Anda dapat menjelajahi website Kiyuti Bookstore secara langsung melalui browser Anda. Anda akan dapat melihat katalog buku, fitur pencarian, dan testimonial, serta menikmati pengalaman berbelanja buku online.

### Tautan Gitthub Pages
Website Kiyuti Bookstore yang telah dibuat dapat diakses melalui GitHub Pages dengan menggunakan tautan berikut:
```teks
https://kirana0219.github.io/Kiyuti-Bookstore-Project-UAS/
```


