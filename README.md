# DIFOSS Holding Mobile Application - Feature & Architecture Specifications

Dokumentasi hasil riset komprehensif dan spesifikasi rekayasa perangkat lunak untuk pembuatan aplikasi mobile resmi [DIFOSS Holding](https://holding.setiadifoss.org/).

## Executive Summary
* [Proposed Features - Executive Summary & Prioritization Matrix](proposed-features-summary.md)
  * Matriks prioritas (P0/P1/P2), kelompok target pengguna, nilai manfaat bisnis, dan peta jalan implementasi 3 fase.

---

## 1. Research & Overview
* [features/01-company-overview-and-research.md](features/01-company-overview-and-research.md)
  * Sasaran pengguna institusi, cakupan domain bisnis (SLiMS, OJS, EPrints, DSpace, CollectiveAccess, keamanan Wazuh), serta daftar mitra kampus.

---

## 2. Existing Features (Parity with Website)
Fitur-fitur yang mereplikasi dan mengoptimalkan fungsi portal web saat ini ke dalam antarmuka mobile iOS dan Android:

* [features/02-feature-auth-and-account.md](features/02-feature-auth-and-account.md)
  * Masuk akun aman, manajemen sesi, profil instansi pengguna, dan pemulihan kata sandi.
* [features/03-feature-services-catalog.md](features/03-feature-services-catalog.md)
  * Instalasi sistem, migrasi data, pengerasan keamanan, pelatihan, dan pengajuan konsultasi kustom.
* [features/04-feature-shop-and-ecommerce.md](features/04-feature-shop-and-ecommerce.md)
  * Paket starter (SLiMS, OJS, EPrints, CollectiveAccess), tema responsif, keranjang, dan pemesanan.
* [features/05-feature-projects-portfolio.md](features/05-feature-projects-portfolio.md)
  * Studi kasus proyek institusi (SilkRoad ScholarRank, IAIN Ponorogo, IJASEIT, Umsida).
* [features/06-feature-news-and-articles.md](features/06-feature-news-and-articles.md)
  * Pengumuman kegiatan pelatihan (DIFOSS Creative Hub), buletin keamanan siber, dan pembaca artikel.
* [features/07-feature-company-profile-faq-contact.md](features/07-feature-company-profile-faq-contact.md)
  * Profil perusahaan, tanya jawab umum (FAQ) interaktif, tombol panggil hotline 24/7, email, dan peta kantor.

---

## 3. New Features (Mobile-First / Value-Add)
Fitur-fitur yang belum ada di portal web saat ini, dirancang khusus untuk penggunaan mobile guna meningkatkan retensi dan kenyamanan klien institusional:

* [features/08-new-feature-support-ticketing.md](features/08-new-feature-support-ticketing.md)
  * Pengajuan tiket aduan dengan lampiran tangkapan layar/log, pemantauan SLA, balasan tim teknis, dan eskalasi WhatsApp.
* [features/09-new-feature-push-notifications.md](features/09-new-feature-push-notifications.md)
  * Notifikasi instan celah eksploitasi keamanan darurat (OJS/SLiMS), pembaruan tiket, dan jadwal pemeliharaan server.
* [features/10-new-feature-infrastructure-health-monitor.md](features/10-new-feature-infrastructure-health-monitor.md)
  * Pemantauan status aktif domain (HTTP 200 ping), hitung mundur masa berlaku sertifikat SSL, dan status pencadangan otomatis.
* [features/11-new-feature-payment-and-invoicing.md](features/11-new-feature-payment-and-invoicing.md)
  * Integrasi Virtual Account Bank lokal, QRIS, unduhan dokumen faktur resmi berformat PDF, dan kuitansi pembayaran.
* [features/12-new-feature-digital-asset-vault.md](features/12-new-feature-digital-asset-vault.md)
  * Pusat unduhan berkas tema/starter kit yang telah dibeli, manajemen kunci lisensi domain, dan notifikasi rilis versi baru.
* [features/13-new-feature-offline-and-caching.md](features/13-new-feature-offline-and-caching.md)
  * Penyimpanan cache lokal untuk panduan teknis dan antrean pengiriman formulir saat berada di ruang server tanpa sinyal.
* [features/14-new-feature-mobile-security-biometrics.md](features/14-new-feature-mobile-security-biometrics.md)
  * Autentikasi biometrik (Sidik Jari / Face ID), enkripsi keystore perangkat keras, SSL pinning, dan deteksi root/jailbreak.

---

## 4. Technical Architecture
* [features/15-technical-architecture-and-api-spec.md](features/15-technical-architecture-and-api-spec.md)
  * Diagram arsitektur sistem, rekomendasi teknologi lintas platform (Flutter / React Native), dan spesifikasi titik akhir (endpoints) REST API.
