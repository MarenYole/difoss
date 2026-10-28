# Jadwal Kerja & Timeline Mingguan Proyek (November - Maret)

Dokumentasi jadwal kerja mingguan (*Gantt Chart / Project Timeline*) untuk pelaksanaan **Project Work Perancangan dan Pengembangan Aplikasi Mobile DIFOSS Holding** bersama mitra **CV. TRENDLY**, Program Studi Teknik Informatika, Fakultas Ilmu Komputer, Universitas Pamulang.

---

## 1. Identitas Proyek & Pembagian Peran Tim

* **Judul Proyek**: Perancangan dan Pengembangan Aplikasi Mobile DIFOSS Holding
* **Mitra Industri**: CV. TRENDLY
* **Lokasi Pelaksanaan**: Jl. Kavling Polri RT 01/RW 02 No. 83B, Kelurahan Perigi Baru, Kecamatan Pondok Aren, Kota Tangerang Selatan, Banten
* **Waktu Penyelesaian**: 5 Bulan (November s.d. Maret - Total 20 Minggu)
* **Susunan Tim Pengembang & Spesialisasi Elemen**:
  1. **Jusuf Herlambang** (NIM: 231011401409) -> **Backend Specialist** (REST API, Layanan Server, Keamanan & Integrasi Sistem Pihak Ketiga)
  2. **Abdyasya Ratzinger Kahulubi** (NIM: 231011400896) -> **Frontend Specialist** (Antarmuka Mobile App, UI/UX, Autentikasi Biometrik & State Management)
  3. **Naufal Akmal Maulana** (NIM: 231011402650) -> **Database Specialist** (Arsitektur Basis Data/ERD, DDL/DML, Optimasi Query, Seeder & Relasi Data)

---

## 2. Matriks 12 Elemen Jadwal Kerja Mingguan (Gantt Chart)

> **Keterangan Penanda:**  
> Simbol `[x]` menandakan pelaksanaan aktif kegiatan pada minggu yang bersangkutan.  
> Kolom **I, II, III, IV** mewakili **Minggu ke-1 sampai Minggu ke-4** pada masing-masing bulan.

| No | Elemen Kegiatan / Pekerjaan | Penanggung Jawab (PIC) | November | | | | Desember | | | | Januari | | | | Februari | | | | Maret | | | |
|:--:|:---|:---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| | | | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** | **I** | **II** | **III** | **IV** |
| 1 | **Analisis Kebutuhan & Perencanaan Sistem** | Bersama (Tim PW) | [x] | [x] | [x] | | | | | | | | | | | | | | | | | |
| 2 | **Perancangan Basis Data & Arsitektur ERD** | Naufal (Database) | | | [x] | [x] | [x] | | | | | | | | | | | | | | | |
| 3 | **Perancangan UI/UX & Wireframing Mobile App** | Abdiyasa (Frontend) | | | | [x] | [x] | [x] | | | | | | | | | | | | | | |
| 4 | **Implementasi Basis Data & Optimasi Query** | Naufal (Database) | | | | | [x] | [x] | [x] | | | | | | | | | | | | | |
| 5 | **Pengembangan REST API & Layanan Backend Inti** | Jusuf (Backend) | | | | | | [x] | [x] | [x] | [x] | | | | | | | | | | | |
| 6 | **Pengembangan Antarmuka & Navigasi Mobile Frontend** | Abdiyasa (Frontend) | | | | | | | [x] | [x] | [x] | [x] | | | | | | | | | | |
| 7 | **Pengembangan Fitur Transaksi, E-Commerce & Invoicing** | Jusuf (Backend) & Abdiyasa (Frontend) | | | | | | | | | [x] | [x] | [x] | [x] | | | | | | | | |
| 8 | **Pengembangan Sistem Tiket Bantuan & Monitoring Infrastruktur** | Jusuf (Backend) & Naufal (Database) | | | | | | | | | | | [x] | [x] | [x] | [x] | | | | | | |
| 9 | **Pengembangan Layanan Notifikasi, Digital Vault & Caching Offline** | Abdiyasa (Frontend) & Jusuf (Backend) | | | | | | | | | | | | | [x] | [x] | [x] | | | | | |
| 10 | **Integrasi Keseluruhan Sistem & Pengujian Fungsional** | Bersama (Tim PW) | | | | | | | | | | | | | | | [x] | [x] | [x] | | | |
| 11 | **Pengujian Keamanan, Kompatibilitas & UAT Mitra** | Bersama & CV. TRENDLY | | | | | | | | | | | | | | | | | [x] | [x] | [x] | |
| 12 | **Dokumentasi, Build Release, Serah Terima & Pelaporan** | Bersama (Tim PW) | | | | | | | | | | | | | | | | | | [x] | [x] | [x] |

---

## 3. Rincian Deskripsi 12 Elemen Pekerjaan

1. **Elemen 1: Analisis Kebutuhan & Perencanaan Sistem (PIC: Bersama - Tim PW)**
   - Waktu: November Minggu I - III
   - Uraian: Observasi alur bisnis portal web DIFOSS eksisting, wawancara kebutuhan mitra CV. TRENDLY, perumusan kebutuhan fungsional dan nonfungsional, serta penyusunan Dokumen KAK dan SKPL.

2. **Elemen 2: Perancangan Basis Data & Arsitektur ERD (PIC: Naufal - Database)**
   - Waktu: November Minggu III - Desember Minggu I
   - Uraian: Pemodelan struktur data relasional untuk 11 modul aplikasi (Pengguna/Auth, Layanan, Toko Digital, Portofolio, Berita, Tiket, Notifikasi, Monitoring, Invoicing, Asset Vault, dan Offline), normalisasi tabel, serta pembuatan diagram ERD terpadu.

3. **Elemen 3: Perancangan UI/UX & Wireframing Mobile App (PIC: Abdiyasa - Frontend)**
   - Waktu: November Minggu IV - Desember Minggu II
   - Uraian: Perancangan user flow navigasi, sketsa wireframe (low-fidelity), pembangunan design system (palet warna, komponen input/tombol), dan pembuatan prototipe interaktif high-fidelity di Figma untuk validasi bersama mitra.

4. **Elemen 4: Implementasi Basis Data & Optimasi Query (PIC: Naufal - Database)**
   - Waktu: Desember Minggu I - III
   - Uraian: Eksekusi DDL migrasi tabel basis data pada server, pembuatan indexing untuk query frekuensi tinggi, data seeder awal (katalog layanan, master data produk), dan perumusan relasi integritas referensial.

5. **Elemen 5: Pengembangan REST API & Layanan Backend Inti (PIC: Jusuf - Backend)**
   - Waktu: Desember Minggu II - Januari Minggu I
   - Uraian: Setup framework backend, implementasi autentikasi JWT aman, role-based access control (RBAC: Admin, Klien, Staf), manajemen sesi login, serta endpoint dasar akun dan profil instansi.

6. **Elemen 6: Pengembangan Antarmuka & Navigasi Mobile Frontend (PIC: Abdiyasa - Frontend)**
   - Waktu: Desember Minggu III - Januari Minggu II
   - Uraian: Setup framework mobile (Flutter/React Native), implementasi autentikasi biometrik (Fingerprint/Face ID), konfigurasi keystore lokal, state management, dan pembangunan layout antarmuka profil serta katalog layanan.

7. **Elemen 7: Pengembangan Fitur Transaksi, E-Commerce & Invoicing (PIC: Jusuf - Backend & Abdiyasa - Frontend)**
   - Waktu: Januari Minggu I - IV
   - Uraian: Implementasi etalase toko digital starter kit (SLiMS/OJS), alur keranjang belanja, integrasi payment gateway (Virtual Account Bank & QRIS), serta generator dokumen faktur resmi institusi format PDF lengkap dengan kalkulasi PPN 11%.

8. **Elemen 8: Pengembangan Sistem Tiket Bantuan & Monitoring Infrastruktur (PIC: Jusuf - Backend & Naufal - Database)**
   - Waktu: Januari Minggu III - Februari Minggu II
   - Uraian: Pembuatan modul ticketing gangguan teknis (unggah screenshot/log, penentuan prioritas, eskalasi penanganan), serta modul pemantauan uptime server klien (ping HTTP 200) dan hitung mundur sertifikat SSL.

9. **Elemen 9: Pengembangan Layanan Notifikasi, Digital Vault & Caching Offline (PIC: Abdiyasa - Frontend & Jusuf - Backend)**
   - Waktu: Februari Minggu I - III
   - Uraian: Integrasi Firebase Cloud Messaging (FCM) untuk siaran peringatan celah keamanan OJS/SLiMS, implementasi brankas aset digital terenkripsi (unduhan installer/tema dan lisensi domain), serta modul luring (*offline mode*) berbasis local storage SQLite/Hive.

10. **Elemen 10: Integrasi Keseluruhan Sistem & Pengujian Fungsional (PIC: Bersama - Tim PW)**
    - Waktu: Februari Minggu III - Maret Minggu I
    - Uraian: Integrasi menyeluruh antara antarmuka mobile, backend REST API, database, payment gateway, dan push service; pelaksanaan pengujian fungsional modul (*Black Box Testing*).

11. **Elemen 11: Pengujian Keamanan, Kompatibilitas & UAT Mitra (PIC: Bersama & CV. TRENDLY)**
    - Waktu: Maret Minggu I - III
    - Uraian: Pengujian keamanan sesi (SSL pinning, keystore, token expiry), uji performa lintas perangkat Android/iOS multi-resolusi, pengujian penerimaan pengguna (*User Acceptance Testing*) bersama mitra CV. TRENDLY, serta penuntasan perbaikan galat (*bug fixing*).

12. **Elemen 12: Dokumentasi, Build Release, Serah Terima & Pelaporan (PIC: Bersama - Tim PW)**
    - Waktu: Maret Minggu II - IV
    - Uraian: Penyusunan Buku Panduan Pengguna (*User Manual Book* untuk klien dan administrator), *build final release* aplikasi (APK/AAB dan iOS package), penyusunan Laporan Akhir Project Work, serah terima hasil proyek, dan penandatanganan Berita Acara bersama CV. TRENDLY.
