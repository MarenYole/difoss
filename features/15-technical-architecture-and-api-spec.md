# Technical Architecture & API Integration Specification

## 1. Arsitektur Tingkat Tinggi
Aplikasi mobile terhubung ke layanan backend DIFOSS melalui antarmuka REST API JSON yang terenkripsi dan terlindungi.

```
+-------------------------------------------------------+
|                   Mobile Client                       |
|           (Flutter / React Native UI)                 |
+-------------------------------------------------------+
                           |
                     HTTPS / TLS 1.3
                    (dengan SSL Pinning)
                           |
+-------------------------------------------------------+
|              Cloudflare WAF / Reverse Proxy           |
+-------------------------------------------------------+
                           |
+-------------------------------------------------------+
|             DIFOSS REST API Gateway                   |
|        (CodeIgniter / Laravel / Node.js API)          |
+-------------------------------------------------------+
         |                 |                  |
+-----------------+ +---------------+ +-----------------+
| Basis Data MySQL| | S3 / MinIO    | | Midtrans/Xendit |
| (Akun, Pesanan, | | (Faktur PDF,  | | (Virtual Acct,  |
|  Tiket, Berita) | |  Tema, Log)   | |  QRIS Gateway)  |
+-----------------+ +---------------+ +-----------------+
```

## 2. Rekomendasi Teknologi (Tech Stack)
* **Framework**: Flutter (Dart) atau React Native (TypeScript) untuk kemudahan pemeliharaan basis kode gabungan iOS dan Android.
* **Manajemen State**:
  * Flutter: Riverpod atau Bloc.
  * React Native: Zustand atau Redux Toolkit.
* **Jaringan & Komunikasi Data**: Dio (Flutter) atau Axios (React Native) dengan interceptor untuk penyegaran token otomatis dan penanganan galat.
* **Penyimpanan Lokal**: Hive / SQLite / WatermelonDB untuk penyimpanan sementara berita, daftar FAQ, dan draf tiket.
* **Notifikasi Siaran**: Firebase Cloud Messaging (FCM) dan Apple Push Notification Service (APNs).
* **SDK Pembayaran**: Midtrans Mobile SDK atau Webview Gateway terintegrasi untuk Virtual Account dan QRIS.

## 3. Rincian Titik Akhir API (API Endpoints)

### Otentikasi & Pengguna
* `POST /api/v1/auth/login` - Otentikasi nama pengguna dan kata sandi; menghasilkan token akses dan refresh berbasis JWT.
* `POST /api/v1/auth/refresh` - Memperbarui token akses yang kedaluwarsa.
* `POST /api/v1/auth/forgot-password` - Permintaan tautan pemulihan kata sandi.
* `GET /api/v1/user/profile` - Mengambil informasi profil pengguna dan peran instansi.

### Layanan & Konsultasi
* `GET /api/v1/services` - Mengambil daftar seluruh kategori layanan.
* `GET /api/v1/services/{id}` - Rincian layanan, cakupan pengerjaan, dan prasyarat.
* `POST /api/v1/services/inquire` - Mengirim formulir pengajuan konsultasi.

### Produk Toko & Pemesanan
* `GET /api/v1/products` - Mengambil daftar paket produk dengan penyaringan harga dan kategori.
* `GET /api/v1/products/{id}` - Spesifikasi paket produk terperinci.
* `POST /api/v1/orders/checkout` - Membuat transaksi pesanan baru.
* `GET /api/v1/orders/history` - Riwayat transaksi masa lalu dan yang sedang diproses.
* `GET /api/v1/orders/{id}/invoice` - Mengunduh dokumen faktur resmi berformat PDF.

### Pusat Bantuan & Tiket (Fitur Baru)
* `GET /api/v1/tickets` - Mengambil daftar tiket bantuan milik akun/kampus.
* `POST /api/v1/tickets` - Membuat tiket aduan baru dengan lampiran berkas (multipart/form-data).
* `GET /api/v1/tickets/{id}/thread` - Mengambil riwayat obrolan dan balasan di dalam tiket.
* `POST /api/v1/tickets/{id}/reply` - Mengirim tanggapan balasan pada tiket yang aktif.

### Pemantauan Infrastruktur Kampus (Fitur Baru)
* `GET /api/v1/monitor/status` - Mengambil status terkini ketersediaan domain dan masa aktif SSL instansi.

### Konten Informasi & Edukasi
* `GET /api/v1/articles` - Berita, pengumuman lokakarya, dan panduan keamanan dengan pagination.
* `GET /api/v1/articles/{id}` - Isi lengkap artikel disertai penambahan angka pembaca.
* `GET /api/v1/projects` - Portofolio studi kasus proyek institusi.
* `GET /api/v1/faq` - Daftar tanya jawab umum berdasarkan kategori.
