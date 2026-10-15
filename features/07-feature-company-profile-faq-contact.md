# Feature Specification: Company Profile, FAQ & Direct Contact

## Status
* **Sumber Asal**: Kesetaraan langsung dengan portal web ([/page/detail/about-us](https://holding.setiadifoss.org/page/detail/about-us), [/page/detail/faq](https://holding.setiadifoss.org/page/detail/faq), [/hubungi](https://holding.setiadifoss.org/hubungi))
* **Prioritas**: Menengah / P1

## Ringkasan Fitur
Menyajikan informasi rekam jejak perusahaan, indikator kredibilitas, logo mitra institusi, jawaban atas pertanyaan umum (FAQ), dan saluran komunikasi langsung dengan tim DIFOSS.

## Kebutuhan Fungsional
1. **Layar Tentang Kami (About Us)**
   * Sejarah perusahaan sejak tahun 2013 dan visi siklus hidup informasi digital.
   * Pilar kompetensi utama: Ilmu Perpustakaan & Informasi, Publikasi Ilmiah Akademik, serta Infrastruktur & Keamanan TI.
   * Galeri logo mitra institusi terpercaya (Perpusnas, UIII, Trisakti, UMN, Untirta, Umsida, Sorong).
2. **Bagian Pusat Bantuan & Tanya Jawab (FAQ)**
   * Model akordeon yang dapat dibuka-tutup untuk menghemat ruang layar.
   * Kategori topik: Prosedur Migrasi, Ketentuan Lisensi, Proteksi Keamanan, Perjanjian Layanan (SLA), dan Metode Pembayaran.
   * Kolom pencarian pertanyaan dengan pemfilteran teks secara langsung (real-time).
3. **Layar Hubungi Kami (Contact Us)**
   * Kartu kontak langsung:
     * Hotline 24/7: +62 812-8269-5757 (sekali sentuh langsung membuka panggilan telepon).
     * Email: info@setiadifoss.org (sekali sentuh langsung membuka aplikasi email).
     * Lokasi Kantor: Tangerang, Banten (sekali sentuh langsung membuka rute di Google Maps).
   * Formulir Pengiriman Pesan:
     * Kolom: Nama Lengkap, Alamat Email, Subjek Pesan, Isi Pesan.
     * Perlindungan kode keamanan/captcha ringan.
     * Pengiriman asinkron dengan notifikasi umpan balik berhasil.
