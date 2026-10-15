# Feature Specification: Client Infrastructure Health Monitor

## Status
* **Sumber Asal**: Fitur Baru (Mobile-First / Nilai Tambah, belum ada di website saat ini)
* **Prioritas**: Menengah / P1 (Layanan Premium Berbasis Kontrak SLA)

## Latar Belakang & Kebutuhan
Klien perguruan tinggi yang berada di bawah kontrak pemeliharaan aktif DIFOSS (misalnya hosting jurnal kampus OJS atau SLiMS) sering merasa khawatir jika layanannya tidak dapat diakses di masa krusial akreditasi atau tenggat pengiriman naskah. Dasbor pemantau status di smartphone menjadikan aplikasi DIFOSS sebagai alat kerja penting harian.

## Metrik Utama yang Dipantau
1. **Status Ketersediaan Domain (Uptime Ping)**
   * Pemeriksaan HTTP/HTTPS berkala setiap 5 menit ke domain kampus klien (contoh: `jurnal.univ.ac.id`, `repository.univ.ac.id`).
   * Indikator status: `Online (200 OK)`, `Lambat / Menurun (>3s)`, `Mati / Gangguan (5xx / Timeout)`.
2. **Kesehatan Sertifikat Keamanan SSL / TLS**
   * Jumlah hari tersisa sebelum sertifikat SSL kedaluwarsa.
   * Peringatan otomatis jika masa aktif tersisa kurang dari 14 hari.
3. **Status Pencadangan Data (Automated Backup)**
   * Catatan waktu dan status keberhasilan pencadangan basis data dan aset digital di server cadangan off-site.
4. **Ringkasan Pemindaian Keamanan**
   * Tanggal pemeriksaan kerentanan terakhir dan status perlindungan WAF Cloudflare.

## Kebutuhan Fungsional
* **Widget Dasbor Status Institusi**: Kartu visual ringkas yang menampilkan ringkasan status seluruh sistem kampus yang terdaftar.
* **Riwayat Insiden Gangguan**: Catatan riwayat insiden sistem mati di masa lalu beserta durasi dan catatan penanganannya.
* **Laporkan Insiden Instan**: Tombol cepat "Laporkan Gangguan" yang langsung mengisi domain yang mati ke dalam pembuatan tiket bantuan teknis.
