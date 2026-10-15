# Proposed Mobile App Features - Executive Summary

## 1. Gambaran Umum
Dokumen ini merangkum seluruh cakupan fitur yang diusulkan untuk pembangunan **Aplikasi Mobile DIFOSS Holding**. Fitur-fitur ini dibagi menjadi dua kategori strategis:
1. **Fitur Kesetaraan Web (Website Parity)**: Fitur inti yang diadaptasi dari portal web [holding.setiadifoss.org](https://holding.setiadifoss.org/) dengan penyesuaian tata letak dan kenyamanan penggunaan perangkat mobile.
2. **Fitur Khusus Mobile (Mobile-First / Nilai Tambah)**: Kemampuan baru yang dirancang untuk menjadikan aplikasi ini sebagai sarana kerja harian yang esensial bagi tim TI kampus, pengelola jurnal, dan pustakawan.

---

## 2. Matriks Perbandingan & Prioritas Fitur

| ID | Nama Fitur | Kategori | Prioritas | Target Pengguna | Nilai Manfaat Utama | Tautan Dokumen Spesifikasi |
|---|---|---|---|---|---|---|
| F-01 | Authentication & User Profile | Kesetaraan Web | P0 (Wajib Ada) | Semua Pengguna | Keamanan identitas akun dan asosiasi institusi | [features/02-feature-auth-and-account.md](features/02-feature-auth-and-account.md) |
| F-02 | Services Catalog & Inquiry | Kesetaraan Web | P0 (Wajib Ada) | Calon Klien / Mitra | Saluran perolehan calon proyek institusi | [features/03-feature-services-catalog.md](features/03-feature-services-catalog.md) |
| F-03 | Digital Shop & E-Commerce | Kesetaraan Web | P0 (Wajib Ada) | Pengadaan Kampus | Pembelian langsung starter kit dan tema | [features/04-feature-shop-and-ecommerce.md](features/04-feature-shop-and-ecommerce.md) |
| F-04 | Projects & Portfolio | Kesetaraan Web | P1 (Perlu Ada) | Calon Klien / Pimpinan | Bukti kredibilitas dan rujukan studi kasus | [features/05-feature-projects-portfolio.md](features/05-feature-projects-portfolio.md) |
| F-05 | News, Articles & Workshops | Kesetaraan Web | P1 (Perlu Ada) | Komunitas Akademik | Keterlibatan komunitas dan pendaftaran pelatihan | [features/06-feature-news-and-articles.md](features/06-feature-news-and-articles.md) |
| F-06 | Company Profile & FAQ | Kesetaraan Web | P1 (Perlu Ada) | Semua Pengguna | Informasi profil dan jawaban mandiri instan | [features/07-feature-company-profile-faq-contact.md](features/07-feature-company-profile-faq-contact.md) |
| F-07 | Support Ticketing System | Fitur Baru Mobile | P0 (Wajib Ada) | Klien Aktif / Admin TI | Kepatuhan SLA dan penanganan insiden cepat | [features/08-new-feature-support-ticketing.md](features/08-new-feature-support-ticketing.md) |
| F-08 | Push Notifications & Security Alerts | Fitur Baru Mobile | P0 (Wajib Ada) | Sysadmin / Editor | Peringatan dini eksploitasi celah OJS/SLiMS | [features/09-new-feature-push-notifications.md](features/09-new-feature-push-notifications.md) |
| F-09 | Infrastructure Health Monitor | Fitur Baru Mobile | P1 (Perlu Ada) | Pengelola TI Kampus | Pemantauan waktu aktif (uptime) dan sertifikat SSL | [features/10-new-feature-infrastructure-health-monitor.md](features/10-new-feature-infrastructure-health-monitor.md) |
| F-10 | Payment Gateway & Invoicing | Fitur Baru Mobile | P0 (Wajib Ada) | Staf Keuangan Kampus | Otomasi Virtual Account/QRIS dan invoice resmi PDF | [features/11-new-feature-payment-and-invoicing.md](features/11-new-feature-payment-and-invoicing.md) |
| F-11 | Digital Asset Vault & Licenses | Fitur Baru Mobile | P1 (Perlu Ada) | Pembeli Paket | Unduhan paket berkas dan pengelolaan kunci lisensi | [features/12-new-feature-digital-asset-vault.md](features/12-new-feature-digital-asset-vault.md) |
| F-12 | Offline Mode & Caching | Fitur Baru Mobile | P2 (Pelengkap) | Teknisi di Lapangan | Akses panduan saat berada di ruang server | [features/13-new-feature-offline-and-caching.md](features/13-new-feature-offline-and-caching.md) |
| F-13 | Biometrics & Mobile Security | Fitur Baru Mobile | P0 (Wajib Ada) | Semua Pengguna | Keamanan kredensial setara perangkat keras | [features/14-new-feature-mobile-security-biometrics.md](features/14-new-feature-mobile-security-biometrics.md) |

---

## 3. Ringkasan Tingkat Tinggi Berdasarkan Kelompok Fitur

### Kelompok A: Transaksi & Pengadaan Institusi (F-02, F-03, F-10, F-11)
* **Tujuan**: Mempermudah perguruan tinggi dan instansi membeli paket layanan, starter kit, serta tema secara praktis.
* **Fungsi Utama**:
  * Eksplorasi dan pemesanan paket siap pakai (SLiMS, OJS, EPrints, CollectiveAccess).
  * Pembayaran terintegrasi Virtual Account Bank (BCA, Mandiri, BNI, BRI) dan QRIS.
  * Faktur resmi institusi berformat PDF lengkap dengan kalkulasi PPN 11% dan generator Pro-Forma Invoice.
  * Gudang digital terlindungi untuk mengunduh paket berkas zip dan pengelolaan lisensi domain.

### Kelompok B: Layanan Pemeliharaan, SLA & Operasional (F-07, F-08, F-09)
* **Tujuan**: Memberikan pendampingan teknis dan jaminan keandalan sistem yang melampaui kemampuan web saat ini.
* **Fungsi Utama**:
  * Pengajuan tiket gangguan dengan lampiran foto bukti galat dan eskalasi langsung ke WhatsApp.
  * Dasbor pantau ketersediaan sistem (uptime HTTP 200) dan hitung mundur kedaluwarsa SSL domain kampus.
  * Siaran notifikasi instan terkait celah keamanan siber darurat (misal: penangkal injeksi judi online/slot gacor pada OJS).

### Kelompok C: Kredibilitas, Komunitas & Edukasi (F-04, F-05, F-06)
* **Tujuan**: Membangun kepercayaan mitra serta mendorong partisipasi dalam program pelatihan DIFOSS.
* **Fungsi Utama**:
  * Portofolio studi kasus bersama mitra kampus terkemuka (Perpusnas, UIII, Trisakti, Umsida).
  * Alur berita dan pendaftaran kegiatan workshop DIFOSS Creative Hub.
  * Tanya jawab umum (FAQ) dan panggilan darurat satu sentuhan ke hotline 24/7 (+62 812-8269-5757).

### Kelompok D: Fondasi Keamanan & Performa Mobile (F-01, F-12, F-13)
* **Tujuan**: Menjamin keamanan akses data institusi dan kecepatan aplikasi saat digunakan.
* **Fungsi Utama**:
  * Masuk cepat menggunakan biometrik (Sidik Jari / Face ID) dengan perlindungan hardware keystore.
  * Pengelolaan sesi JWT dengan proteksi SSL Pinning guna mencegah intersepsi data.
  * Penyimpanan lokal (caching) berbasis SQLite/Hive dan antrean sinkronisasi data otomatis saat offline.

---

## 4. Rencana Tahapan Rilis (Roadmap)

### Fase 1: Peluncuran MVP (Minggu 1 - 6)
* Fokus pada fitur wajib berprioritas P0:
  * Autentikasi Akun & Biometrik ([F-01](features/02-feature-auth-and-account.md), [F-13](features/14-new-feature-mobile-security-biometrics.md))
  * Katalog Layanan & Konsultasi ([F-02](features/03-feature-services-catalog.md))
  * Toko Digital & Pemesanan Paket ([F-03](features/04-feature-shop-and-ecommerce.md))
  * Gerbang Pembayaran Dasar & Faktur ([F-10](features/11-new-feature-payment-and-invoicing.md))
  * Sistem Tiket Aduan Gangguan ([F-07](features/08-new-feature-support-ticketing.md))
  * Notifikasi Siaran untuk Tiket & Peringatan Keamanan ([F-08](features/09-new-feature-push-notifications.md))

### Fase 2: Konten & Penguatan Ekosistem (Minggu 7 - 10)
* Implementasi fitur prioritas P1:
  * Studi Kasus Portofolio Proyek ([F-04](features/05-feature-projects-portfolio.md))
  * Berita, Artikel & Registrasi Workshop ([F-05](features/06-feature-news-and-articles.md))
  * Gudang Aset Digital & Lisensi Mandiri ([F-11](features/12-new-feature-digital-asset-vault.md))
  * Profil Perusahaan & FAQ Interaktif ([F-06](features/07-feature-company-profile-faq-contact.md))

### Fase 3: Layanan Pemantauan Lanjutan & Fitur Offline (Minggu 11 - 14)
* Fitur lanjutan dan penyempurnaan:
  * Pemantau Kesehatan Infrastruktur Kampus ([F-09](features/10-new-feature-infrastructure-health-monitor.md))
  * Mode Offline & Penyimpanan Cache Panduan ([F-12](features/13-new-feature-offline-and-caching.md))
