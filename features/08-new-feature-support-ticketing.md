# Feature Specification: Client Support & Maintenance Ticketing System

## Status
* **Sumber Asal**: Fitur Baru (Mobile-First / Nilai Tambah, belum ada di website saat ini)
* **Prioritas**: Utama / P0 (sangat krusial untuk retensi klien institusional)

## Latar Belakang & Kebutuhan
DIFOSS Holding menyediakan layanan pemeliharaan sistem penting institusi (SLiMS, OJS, EPrints). Saat ini, portal web hanya memiliki formulir kontak biasa. Ketika jurnal ilmiah atau repositori kampus mengalami gangguan server atau galat (error) di tengah proses akreditasi, pengelola kampus membutuhkan sistem tiket pengaduan yang cepat, terstruktur, dan memiliki riwayat audit jelas.

## Kebutuhan Pengguna (User Stories)
* Sebagai pengelola jurnal, saya ingin melaporkan kegagalan pengiriman naskah di OJS disertai tangkapan layar galat agar tim teknis DIFOSS dapat segera memperbaikinya.
* Sebagai pimpinan TI kampus, saya ingin memantau seluruh tiket kendala yang diajukan staf universitas untuk memastikan perjanjian tingkat layanan (SLA) terpenuhi tepat waktu.

## Kebutuhan Fungsional
1. **Pembuatan Tiket Bantuan**
   * Pilihan kategori: Platform (OJS / SLiMS / EPrints / Server / Lainnya).
   * Tingkat urgensi: `Kritis - Layanan Terhenti`, `Tinggi - Performa Menurun`, `Sedang - Gangguan Fitur`, `Rendah - Konsultasi / Permintaan Fitur`.
   * Kolom domain target / tautan sistem yang bermasalah.
   * Judul dan rincian kronologi permasalahan.
   * Lampiran: Pengunggahan foto tangkapan layar, dokumen log galat, atau berkas konfigurasi langsung dari kamera atau penyimpanan smartphone.
2. **Dasbor Tiket & Pelacakan Status**
   * Tab penyaringan status: `Semua`, `Terbuka (Open)`, `Sedang Diproses (In Progress)`, `Menunggu Respon Klien`, `Terselesaikan (Resolved)`, `Ditutup (Closed)`.
   * Tampilan lini masa waktu penanganan tiket oleh tim teknis DIFOSS.
   * Penghitung waktu mundur SLA bagi instansi yang memiliki kontrak layanan prioritas.
3. **Pesan & Percakapan Dalam Tiket (Threading)**
   * Format ruang percakapan berbalas di dalam masing-masing tiket.
   * Tombol aksi cepat "Eskalasi ke WhatsApp" yang langsung menyertakan nomor tiket saat menghubungi narahubung teknis yang bertugas.
4. **Konfirmasi Penyelesaian & Ulasan Layanan**
   * Konfirmasi mandiri oleh pengguna sebelum tiket ditutup secara permanen.
   * Formulir penilaian kepuasan layanan bintang 1 hingga 5 disertai catatan evaluasi.
