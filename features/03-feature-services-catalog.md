# Feature Specification: Services Catalog & Consultation Booking

## Status
* **Sumber Asal**: Kesetaraan langsung dengan portal web ([/services](https://holding.setiadifoss.org/))
* **Prioritas**: Utama / P0

## Ringkasan Fitur
Menampilkan portofolio layanan konsultasi teknis dan rekayasa perangkat lunak institusional dari DIFOSS Holding, memungkinkan klien institusi dan perguruan tinggi mempelajari cakupan solusi serta mengajukan konsultasi langsung melalui perangkat mobile.

## Rincian Katalog Layanan
1. **System Installation & Setup**
   * Instalasi dan konfigurasi Open Journal Systems (OJS), repositori EPrints, dan sistem perpustakaan SLiMS.
   * Optimasi dasar server (PHP, Nginx/Apache, MySQL/MariaDB).
2. **Upgrade & Maintenance**
   * Peningkatan dan migrasi dari OJS 2 lama ke OJS 3 terkini.
   * Optimasi indeks basis data, perbaikan skema, dan kontrak pemeliharaan berkala.
3. **Premium Themes & Plugins**
   * Kustomisasi antarmuka web jurnal/perpustakaan yang modern, responsif, dan ramah pengguna.
   * Pemasangan plugin pendukung (ORCID, CrossRef, indeksasi Google Scholar, integrasi Turnitin).
4. **Server & Database Migration**
   * Migrasi server lokal (on-premise) ke infrastruktur Cloud/VPS.
   * Validasi integritas data dengan jaminan tanpa kehilangan data (zero data loss).
5. **Website Security & Cloudflare Hardening**
   * Perlindungan terhadap serangan, konfigurasi WAF/DNS Cloudflare, sertifikat SSL, dan pencegahan eksploitasi celah keamanan.
6. **Training & Support**
   * Pelatihan teknis bagi pengelola jurnal, penyunting naskah, penelaah, dan pustakawan.
7. **Custom Development**
   * Pengembangan modul/plugin kustom PHP/Python, integrasi API eksternal, dan Single Sign-On (SSO/SAML/OAuth).

## Kebutuhan Fungsional
* **Eksplorasi Katalog**: Tampilan kartu visual dengan ikon, deskripsi ringkas, dan filter kategori.
* **Halaman Rincian Layanan**: Cakupan pekerjaan terperinci, dokumen hasil keluaran (deliverables), prasyarat teknis, dan portofolio terkait.
* **Formulir Pengajuan Konsultasi**:
  * Kolom: Nama Institusi/Kampus, Jenis Layanan yang Dibutuhkan (terpilih otomatis), Nama Narahubung, Nomor Telepon/WhatsApp, Email, Versi Sistem yang Sedang Digunakan, Deskripsi Kebutuhan Proyek.
  * Terkirim langsung ke API backend untuk menjadi tiket prospek konsultasi.
  * Tombol aksi cepat "Konsultasi via WhatsApp" dengan format pesan yang sudah terisi otomatis.
