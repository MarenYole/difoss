# Jadwal Kerja & Timeline Mingguan Proyek (November - Maret)

Dokumentasi jadwal kerja mingguan (*Gantt Chart / Project Timeline*) untuk pelaksanaan **Project Work Perancangan dan Pengembangan Aplikasi Mobile DIFOSS Holding** bersama mitra **CV. TRENDLY**, Program Studi Teknik Informatika, Fakultas Ilmu Komputer, Universitas Pamulang.

---

## 1. Identitas & Periode Proyek
* **Judul Proyek**: Perancangan dan Pengembangan Aplikasi Mobile DIFOSS Holding
* **Mitra Industri**: CV. TRENDLY
* **Lokasi Pelaksanaan**: Jl. Kavling Polri RT 01/RW 02 No. 83B, Kelurahan Perigi Baru, Kecamatan Pondok Aren, Kota Tangerang Selatan, Banten
* **Waktu Penyelesaian**: 5 Bulan (November s.d. Maret - Total 20 Minggu)
* **Tim Pengembang**:
  1. Jusuf Herlambang (NIM: 231011401409) - Lead Developer / Mobile Frontend
  2. Abdyasya Ratzinger Kahulubi (NIM: 231011400896) - Backend & Cloud Integration Specialist
  3. Naufal Akmal Maulana (NIM: 231011402650) - System Analyst, QA & Technical Writer

---

## 2. Matriks Jadwal Kerja Mingguan (Gantt Chart)

> **Keterangan Penanda:**  
> Simbol `[x]` menandakan alokasi pelaksanaan aktif kegiatan pada minggu yang bersangkutan.  
> Kolom **I, II, III, IV** mewakili **Minggu ke-1 sampai Minggu ke-4** pada masing-masing bulan.

| No | Tahapan & Uraian Kegiatan | November | | | | Desember | | | | Januari | | | | Februari | | | | Maret | | | |
|:--:|:---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| | | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** |
| **A** | **TAHAP 1: ANALISIS KEBUTUHAN & PERENCANAAN** | | | | | | | | | | | | | | | | | | | | |
| 1 | Inisiasi proyek, studi literatur, & koordinasi kebutuhan mitra CV. TRENDLY | [x] | | | | | | | | | | | | | | | | | | | |
| 2 | Analisis proses bisnis portal web DIFOSS eksisting & identifikasi kebutuhan sistem mobile | | [x] | [x] | | | | | | | | | | | | | | | | | |
| 3 | Penyusunan Dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) & Kerangka Acuan Kerja (KAK) | | | [x] | [x] | | | | | | | | | | | | | | | | |
| **B** | **TAHAP 2: PERANCANGAN SISTEM & DESAIN UI/UX** | | | | | | | | | | | | | | | | | | | | |
| 4 | Perancangan arsitektur sistem, skema basis data relasional (ERD), & spesifikasi kontrak REST API | | | [x] | [x] | | | | | | | | | | | | | | | | |
| 5 | Pemodelan proses bisnis & alur data sistem (Flowchart, Use Case Diagram, & Sequence Diagram) | | | | [x] | [x] | | | | | | | | | | | | | | | |
| 6 | Perancangan kerangka antarmuka dasar (*Wireframing / Low-Fidelity*) | | | | | [x] | | | | | | | | | | | | | | | |
| 7 | Perancangan antarmuka visual (*High-Fidelity UI Mockup*) & *Design System* di Figma | | | | | [x] | [x] | | | | | | | | | | | | | | |
| 8 | Pembuatan purwarupa interaktif (*Interactive Prototype*) & validasi antarmuka bersama mitra | | | | | | [x] | | | | | | | | | | | | | | |
| **C** | **TAHAP 3: PENGEMBANGAN PERANGKAT LUNAK (IMPLEMENTASI MODUL)** | | | | | | | | | | | | | | | | | | | | |
| 9 | Penyiapan lingkungan pengembangan (*environment setup*), repositori, & *state management* mobile | | | | | | [x] | [x] | | | | | | | | | | | | | |
| 10 | Pengembangan backend REST API dasar, autentikasi (JWT), manajemen profil, & hak akses (RBAC) | | | | | | | [x] | [x] | | | | | | | | | | | | |
| 11 | Implementasi keamanan mobile & autentikasi biometrik (*Fingerprint / Face ID, Keystore*, SSL Pinning) | | | | | | | | [x] | [x] | | | | | | | | | | | |
| 12 | Pengembangan Modul Profil Perusahaan, FAQ, Kontak Darurat 24/7, & Katalog Layanan Konsultasi | | | | | | | | | [x] | [x] | | | | | | | | | | |
| 13 | Pengembangan Modul Toko Digital (*E-Commerce*), Starter Kit (SLiMS/OJS), & Keranjang Belanja | | | | | | | | | | [x] | [x] | | | | | | | | | |
| 14 | Pengembangan Modul Portofolio Proyek Klien & Rubrik Berita / Workshop DIFOSS Creative Hub | | | | | | | | | | | [x] | [x] | | | | | | | | |
| 15 | Pengembangan Modul *Client Support & Maintenance Ticketing System* beserta riwayat penanganan | | | | | | | | | | | | [x] | [x] | | | | | | | |
| 16 | Implementasi *Push Notifications & Security Alerts* (FCM: peringatan celah OJS/SLiMS & status tiket) | | | | | | | | | | | | | [x] | [x] | | | | | | |
| 17 | Integrasi *Payment Gateway* (Virtual Account & QRIS) serta generator *Institutional Invoicing* PDF (PPN 11%) | | | | | | | | | | | | | | [x] | [x] | | | | | |
| 18 | Pengembangan Modul *Client Infrastructure Health Monitor* (pemantauan server, ping HTTP 200, & SSL) | | | | | | | | | | | | | | | [x] | [x] | | | | |
| 19 | Pengembangan Modul *Digital Asset Vault* (brankas unduhan tema/kit terenkripsi & lisensi domain) | | | | | | | | | | | | | | | [x] | [x] | | | | |
| 20 | Pengembangan Modul *Offline Mode & Knowledge Base Caching* (penyimpanan lokal SQLite/Hive & sinkronisasi data) | | | | | | | | | | | | | | | | [x] | [x] | | | |
| **D** | **TAHAP 4: INTEGRASI SISTEM & PENGUJIAN** | | | | | | | | | | | | | | | | | | | | |
| 21 | Integrasi menyeluruh antar-modul (*Front-End Mobile, Backend REST API, Payment Gateway, & Firebase*) | | | | | | | | | | | | | | | | [x] | [x] | | | |
| 22 | Pengujian fungsional (*Black Box Testing*) pada alur transaksi, tiket aduan, dan manajemen lisensi | | | | | | | | | | | | | | | | | [x] | [x] | | |
| 23 | Pengujian performa sistem, kompatibilitas perangkat multi-resolusi Android/iOS, & keamanan enkripsi | | | | | | | | | | | | | | | | | | [x] | [x] | |
| 24 | *User Acceptance Testing* (UAT) bersama pihak CV. TRENDLY serta perbaikan galat (*bug fixing*) | | | | | | | | | | | | | | | | | | [x] | [x] | |
| **E** | **TAHAP 5: DOKUMENTASI, SERAH TERIMA & PELAPORAN** | | | | | | | | | | | | | | | | | | | | |
| 25 | Penyusunan Buku Panduan Pengguna (*User Manual Book*) untuk Klien dan Administrator Sistem | | | | | | | | | | | | | | | | | | [x] | [x] | |
| 26 | *Build final package* aplikasi (berkas APK/AAB Android & paket iOS) serta deployment backend server | | | | | | | | | | | | | | | | | | | [x] | [x] |
| 27 | Penyusunan draf Laporan Akhir Project Work & luaran publikasi/jurnal | | | | | | | | | | | | | | | | | | [x] | [x] | [x] |
| 28 | Evaluasi akhir, serah terima aplikasi, & penandatanganan Berita Acara bersama mitra CV. TRENDLY | | | | | | | | | | | | | | | | | | | | [x] |
| 29 | Finalisasi berkas pelaporan dan persiapan sidang Project Work | | | | | | | | | | | | | | | | | | | | [x] |

---

## 3. Rincian Milestone Bulanan

### Bulan 1: November - Analisis Kebutuhan & Perancangan Arsitektur (Minggu 1 - 4)
* **Minggu 1**: Pertemuan awal (*kick-off*) dengan perwakilan CV. TRENDLY, pengumpulan berkas dan dokumentasi layanan eksisting, serta wawancara pemangku kepentingan.
* **Minggu 2**: Identifikasi kebutuhan fungsional dan nonfungsional, perumusan batasan sistem, dan klasifikasi prioritas fitur (P0/P1/P2).
* **Minggu 3**: Penyusunan dokumen Kerangka Acuan Kerja (KAK) dan perancangan skema basis data (*Entity Relationship Diagram*).
* **Minggu 4**: Pembuatan spesifikasi kontrak REST API, pemodelan diagram alur kerja (*Flowchart*, *Use Case*, dan *Sequence Diagram*).

### Bulan 2: Desember - Desain UI/UX & Fondasi Keamanan (Minggu 5 - 8)
* **Minggu 5**: Perancangan sketsa wireframe (low-fidelity) dan inisiasi *design system* di Figma (palet warna, tipografi, komponen tombol/input).
* **Minggu 6**: Penyusunan purwarupa antarmuka *high-fidelity*, uji coba alur navigasi interaktif, serta review persetujuan desain oleh CV. TRENDLY.
* **Minggu 7**: Inisiasi repositori aplikasi mobile dan backend service; implementasi modul autentikasi dasar (registrasi, login, reset password, dan JWT handling).
* **Minggu 8**: Penguatan keamanan aplikasi mobile (integrasi biometrik Face ID/Fingerprint, penyimpanan aman hardware keystore, dan konfigurasi SSL pinning).

### Bulan 3: Januari - Modul Layanan, E-Commerce, & Sistem Tiket (Minggu 9 - 12)
* **Minggu 9**: Implementasi halaman profil perusahaan, kontak darurat, FAQ dinamis, serta katalog layanan IT lengkap dengan alur reservasi jadwal konsultasi.
* **Minggu 10**: Implementasi modul e-commerce: etalase starter kit (SLiMS, OJS, EPrints, CollectiveAccess), detail spesifikasi paket, dan keranjang belanja.
* **Minggu 11**: Pengembangan modul portofolio proyek (studi kasus instansi kampus) dan rubrik berita/workshop teknologi DIFOSS Creative Hub.
* **Minggu 12**: Pembangunan modul *Support Ticketing System*: pembuatan tiket gangguan teknis, unggah bukti tangkapan layar/log, pemilihan prioritas, dan riwayat penanganan.

### Bulan 4: Februari - Notifikasi, Monitoring, Payment, & Offline Mode (Minggu 13 - 16)
* **Minggu 13**: Integrasi layanan Firebase Cloud Messaging (FCM) untuk siaran peringatan celah keamanan siber OJS/SLiMS dan notifikasi status tiket.
* **Minggu 14**: Integrasi Payment Gateway (Virtual Account Bank & QRIS) serta engine pembuatan faktur resmi PDF instansi lengkap dengan PPN 11%.
* **Minggu 15**: Implementasi dasbor *Client Infrastructure Health Monitor* untuk memantau uptime server (ping HTTP 200) dan hitung mundur kedaluwarsa sertifikat SSL.
* **Minggu 16**: Implementasi *Digital Asset Vault* (brankas unduhan aman tema/starter kit dan pengelolaan lisensi domain) serta *Offline Mode* berbasis caching SQLite/Hive.

### Bulan 5: Maret - Integrasi Penuh, Pengujian, Dokumentasi, & Serah Terima (Minggu 17 - 20)
* **Minggu 17**: Integrasi menyeluruh antara antarmuka mobile, backend REST API, payment gateway, dan notifikasi; pelaksanaan pengujian fungsional *Black Box*.
* **Minggu 18**: Pengujian keamanan sistem, pengujian performa respon jaringan, serta pelaksanaan *User Acceptance Testing* (UAT) bersama mitra CV. TRENDLY.
* **Minggu 19**: Perbaikan catatan evaluasi UAT, penyusunan Buku Panduan Pengguna (*User Manual Book*), dan *build* berkas instalasi rilis (APK/AAB dan paket iOS).
* **Minggu 20**: Finalisasi Dokumen Laporan Akhir Project Work, serah terima aplikasi dan Berita Acara kepada CV. TRENDLY, serta persiapan sidang proyek.

---

## 4. Pembagian Peran dan Tanggung Jawab Tim

* **Jusuf Herlambang (Lead Developer / Mobile Frontend)**
  * Arsitektur front-end mobile dan manajemen state.
  * Implementasi antarmuka pengguna (UI/UX) berdasarkan prototype Figma.
  * Integrasi autentikasi biometrik, keystore lokal, dan pengemasan file rilis instalasi (APK/AAB).
* **Abdyasya Ratzinger Kahulubi (Backend & Cloud Integration Specialist)**
  * Perancangan skema database (ERD) dan manajemen query.
  * Pengembangan endpoint REST API dan keamanan komunikasi data (JWT, HTTPS, SSL Pinning).
  * Integrasi layanan pihak ketiga (Payment Gateway, Firebase Cloud Messaging, dan generator PDF invoice).
* **Naufal Akmal Maulana (System Analyst, QA & Technical Writer)**
  * Analisis kebutuhan sistem dan pemodelan diagram UML (Use Case, Activity, Sequence).
  * Perencanaan dan pelaksanaan skenario pengujian sistem (*Black Box Testing* & koordinasi UAT).
  * Penyusunan dokumentasi proyek: KAK, Buku Panduan Pengguna (*User Manual Book*), dan Laporan Akhir Project Work.
