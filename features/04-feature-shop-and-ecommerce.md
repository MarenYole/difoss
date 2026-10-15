# Feature Specification: Digital Shop & E-Commerce Workflow

## Status
* **Sumber Asal**: Kesetaraan langsung dengan portal web ([/shop](https://holding.setiadifoss.org/shop))
* **Prioritas**: Utama / P0

## Ringkasan Fitur
Memungkinkan pengelola institusi, pustakawan, dan editor melihat katalog, memilih, dan memesan paket instalasi siap pakai (starter kits) serta tema premium yang dikembangkan oleh DIFOSS Holding.

## Katalog Produk yang Tersedia (Data dari Web)
* **EPrints Clean & Responsive Designs**: Rp 5.000.000
* **Starter SLiMS**: Rp 3.000.000
* **Starter EPrints**: Rp 7.000.000
* **Starter OJS**: Rp 3.000.000
* **Starter CA (CollectiveAccess)**: Rp 7.000.000

## Kebutuhan Fungsional

### 1. Daftar Produk & Penyaringan
* Pilihan tampilan grid (kotak) dan list (daftar) yang disesuaikan untuk layar smartphone.
* Menampilkan gambar pratinjau produk, judul paket, harga dalam format Rupiah (IDR), dan rating bintang ulasan.
* Filter berdasarkan platform (OJS, SLiMS, EPrints, CollectiveAccess).
* Fitur pencarian instan berdasarkan kata kunci dengan rekomendasi otomatis.

### 2. Halaman Rincian Produk
* Tangkapan layar resolusi tinggi dengan galeri geser (carousel).
* Penjelasan kelengkapan paket (dokumentasi panduan, durasi pendampingan/support gratis, jasa bantuan instalasi).
* Informasi kompatibilitas versi (contoh: OJS versi 3.3.x, SLiMS 9 Bulian, EPrints 3.4.x).
* Tombol aksi "Tambah ke Keranjang" dan "Pesan Langsung".

### 3. Manajemen Keranjang Belanja
* Lencana keranjang mengambang (floating badge) yang menampilkan jumlah item aktif.
* Halaman keranjang belanja dengan gambar kecil, judul, harga satuan, pengatur kuantitas, dan subtotal.
* Kolom kode voucher / diskon khusus institusi.
* Catatan pesanan (misal: nama domain target atau nama perguruan tinggi pemohon).

### 4. Alur Pembayaran & Pemesanan (Checkout)
* Formulir data penagihan institusi (Nama Universitas/Lembaga, NPWP jika ada, Alamat Resmi, Kontak Bagian Keuangan).
* Pemilihan metode pembayaran (Transfer Bank Manual, Virtual Account, QRIS).
* Layar konfirmasi pesanan dengan ketentuan lisensi dan syarat layanan.
* Layar pelacakan status pesanan lengkap dengan nomor referensi unik.
