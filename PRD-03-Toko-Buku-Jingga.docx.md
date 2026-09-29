 

 

 

 

 

**PRODUCT REQUIREMENT DOCUMENT**

**PRD-03 — Toko Buku Jingga**

Product Requirement Document (PRD) \- Praktik Kelas

 

 

 

 

 

 

 

Landing page profil toko buku independen dengan kurasi dan rekomendasi.

## **1\. Ringkasan**

Toko Buku Jingga adalah toko buku independen yang mengkurasi buku pilihan untuk pembaca umum, pelajar, dan kolektor. Halaman profil ini memperkenalkan koleksi, menampilkan buku terlaris, dan memudahkan pembeli menghubungi toko untuk pemesanan.

## **2\. Latar belakang dan masalah**

Pembeli sering bertanya lewat pesan pribadi tentang stok, kategori, dan rekomendasi. Katalog yang tersebar di unggahan media sosial membuat calon pembeli sulit membandingkan pilihan. Toko kehilangan peluang karena informasi tidak terpusat.

Masalah yang dipecahkan: calon pembeli tidak bisa melihat kategori, buku unggulan, dan cara pemesanan dalam satu tempat yang rapi.

## **3\. Tujuan**

1. Calon pembeli melihat kategori buku yang tersedia.  
2. Calon pembeli melihat buku terlaris dengan informasi yang jelas.  
3. Calon pembeli membaca testimoni pembaca lain.  
4. Calon pembeli bisa menghubungi toko atau melihat promo bundling.

## **4\. Pengguna sasaran**

| Pengguna | Kebutuhan |
| ----- | ----- |
| Pembaca umum | Melihat kategori dan buku terlaris dengan cepat |
| Pelajar yang mencari buku pelajaran | Melihat kategori pelajaran dan paket bundling |
| Kolektor dan pembaca setia | Melihat kurasi dan testimoni pembaca lain |

## **5\. Ruang lingkup**

**Masuk lingkup:** satu halaman statis dengan enam \*section\* dan satu \*footer\*, dibangun per \*section\*, ditayangkan ke Netlify.

**Di luar lingkup:** keranjang belanja, pembayaran, stok real-time, dan akun pembeli.

## **6\. Daftar section**

| No | Section | Isi wajib | Catatan |
| ----- | ----- | ----- | ----- |
| 1 | Hero | Nama toko, kalimat penjelas "Buku pilihan, kurasi jujur", tombol Jelajahi Koleksi | Visual hangat, warna jingga-krem berbasis color palette Gramedia.id (Navy `#1D3A6C`, Jingga `#EE6039`, Krem `#FFF9F5`) |
| 2 | Kategori | Empat kartu kategori: fiksi, nonfiksi, anak, pelajaran. Tiap kartu berisi nama kategori dan jumlah judul contoh | Empat kartu, ikon sederhana |
| 3 | Buku terlaris | Enam buku dengan sampul, judul, penulis, dan harga | Grid 3 kolom desktop, 2 kolom ponsel |
| 4 | Testimoni pembaca | Tiga kutipan pembaca beserta nama dan buku yang dibeli | Menyebut buku yang dibeli |
| 5 | Promo bundling | Tiga paket bundling: Pelajar, Keluarga Membaca, Kolektor. Tiap paket berisi harga bundling, isi paket, dan satu kalimat penjelas | Paket Pelajar ditandai hemat |
| 6 | Kontak | Alamat toko, jam buka, tautan WhatsApp dan media sosial, tautan peta |  |
| 7 | Footer | Hak cipta, tautan kategori, dan jam buka ringkas |  |

## **7\. User stories**

| ID | Sebagai | Saya ingin | Acceptance criteria |
| ----- | ----- | ----- | ----- |
| US-01 | Pembaca umum | Melihat kategori buku yang tersedia | Section Kategori menampilkan empat kartu kategori |
| US-02 | Calon pembeli | Melihat buku terlaris dengan informasi lengkap | Section Buku terlaris menampilkan enam buku dengan sampul, judul, penulis, dan harga |
| US-03 | Pembaca yang membandingkan | Membandingkan paket bundling | Section Promo menampilkan tiga paket dengan harga dan isi |
| US-04 | Pembeli baru | Membaca testimoni pembaca lain | Testimoni menampilkan tiga kutipan beserta nama dan buku |
| US-05 | Pengunjung yang siap membeli | Menghubungi toko | Tautan WhatsApp dan peta bisa dibuka |

## **8\. Alur pengguna**

Buka hero → melihat kategori → melihat buku terlaris → membaca testimoni → membandingkan promo bundling → menghubungi toko.

## **9\. Kriteria visual**

1. **Patokan Utama Color Palette ([Gramedia.id](https://gramedia.id/)):**
   - **Primary Navy Blue (`#1D3A6C` / Biscay):** Warna identitas utama untuk judul section, navigasi, dan elemen penegas.
   - **Accent Flamingo Orange / Jingga (`#EE6039`):** Warna aksen utama toko (Jingga) untuk tombol CTA ("Jelajahi Koleksi"), badge promo, dan link aktif.
   - **Highlight Gold (`#FED66F`):** Bintang ulasan/rating dan aksen paket rekomendasi.
   - **Warm Jingga-Krem Background (`#FFF9F5` / `#F8F9FA`):** Nuansa visual hangat jingga-krem yang bersih dan ramah pembaca.
   - **Surface & Border (`#FFFFFF` & `#E4E7EC`):** Kartu konten putih bersih dengan border tipis elegan dan bayangan lembut.
   - **Teks Utama & Sekunder (`#1D2939` & `#475467`):** Tipografi kontras tinggi yang nyaman dibaca di layar ponsel maupun desktop.
2. Warna hangat jingga-krem yang cocok dengan tema toko buku, konsisten di seluruh *section*.  
3. Sampul buku dengan rasio sama (3:4) dan tipografi yang menenangkan.  
4. Rapi dan responsif di layar ponsel (grid 2 kolom) dan desktop (grid 3 kolom).

## **10\. Kriteria teknis**

9. Dibangun per \*section\* dengan \*prompt\* terpisah.  
10. Minimal tiga \*commit\* dengan pesan yang menyebut bagian, lalu di-\*push\*.  
11. Ditayangkan ke Netlify dengan URL netlify.app.  
12. Bisa menjelaskan satu \*diff\*.

## **11\. Kriteria selesai**

URL bisa dibuka publik tanpa galat, seluruh \*section\* tampil dan rapi di ponsel, \*repositori\* memuat tiga \*commit\*, dan satu \*diff\* bisa dijelaskan.

## **12\. Batasan dan asumsi**

13. Halaman statis, tanpa keranjang dan pembayaran.  
14. Sampul buku memakai gambar contoh.  
15. Promo bundling memakai harga contoh.

## **13\. Risiko**

Halaman yang terlalu ramai bisa membuat pembeli bingung. Mitigasi: tiap \*section\* hanya menampilkan informasi yang ada pada tabel, tidak menambah di luar daftar.