# Feature Specification: Push Notifications & Security Alerts

## Status
* **Sumber Asal**: Fitur Baru (Mobile-First / Belum ada di website saat ini)
* **Prioritas**: Utama / P0

## Latar Belakang & Kebutuhan
Portal web saat ini mengandalkan kunjungan pasif. Aplikasi mobile memungkinkan DIFOSS secara proaktif mengirimkan peringatan dini kepada para administrator kampus mengenai celah keamanan kritis pada platform akademik, jendela pemeliharaan server terjadwal, pembaruan status pesanan, serta balasan tiket bantuan.

## Kategori Notifikasi
1. **Peringatan Keamanan Siber Kritis (Security Bulletins)**
   * Siaran notifikasi mendesak saat ditemukan celah eksploitasi baru pada OJS (contoh: injeksi slot gacor, celah remote code execution) atau SLiMS beserta panduan langkah mitigasi instan.
2. **Pembaruan Tiket Bantuan**
   * Pemberitahuan langsung saat tim teknis DIFOSS memberikan respon atau menyelesaikan kendala pada tiket klien.
3. **Pemberitahuan Pemeliharaan Server (Maintenance)**
   * Notifikasi terjadwal saat sistem klien sedang dalam proses pencadangan (backup), migrasi basis data, atau penambalan server.
4. **Pembaruan Pesanan & Lisensi**
   * Informasi status transaksi produk digital dan penerbitan kunci lisensi baru.
5. **Agenda Pelatihan & Workshop**
   * Pengingat jadwal pelatihan yang diadakan oleh DIFOSS Creative Hub.

## Kebutuhan Fungsional
* **Integrasi Layanan Notifikasi**: Pendaftaran token perangkat saat login pengguna; mendukung APNs (iOS) dan FCM (Android).
* **Pusat Pengaturan Preferensi Notifikasi**: Pengguna dapat mengaktifkan atau menonaktifkan saluran tertentu (misal: mematikan notifikasi promosi, tetapi tetap menyalakan peringatan keamanan kritis).
* **Kotak Masuk Notifikasi Dalam Aplikasi (Notification Inbox)**: Riwayat pesan notifikasi yang telah diterima dengan tanda sudah/belum dibaca.
* **Tautan Langsung (Deep Linking)**: Menekan notifikasi akan langsung membuka layar yang relevan (misal: langsung ke tiket kendala, artikel buletin keamanan, atau rincian pesanan).
