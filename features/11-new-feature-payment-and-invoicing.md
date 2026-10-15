# Feature Specification: In-App Payment Gateway & Institutional Invoicing

## Status
* **Sumber Asal**: Fitur Baru (Mobile-First / Belum ada di website saat ini)
* **Prioritas**: Utama / P0

## Latar Belakang & Kebutuhan
Portal web saat ini belum memiliki integrasi gerbang pembayaran otomatis maupun pembuatan faktur mandiri. Lembaga pendidikan dan instansi pemerintah memiliki aturan birokrasi pengadaan ketat yang mewajibkan ketersediaan invoice formal, pro-forma invoice, dan bukti bayar yang memuat nomor pokok wajib pajak (NPWP).

## Saluran Pembayaran yang Didukung
* **Virtual Account Bank Indonesia**: BCA, Bank Mandiri, BNI, BRI, Permata.
* **QRIS Dinamis**: Tampilan kode QRIS instan di dalam aplikasi dengan waktu hitung mundur.
* **Transfer Bank Manual / Giro Institusi**: Fasilitas unggah bukti setor atau nota transfer dengan verifikasi berkas oleh admin keuangan.

## Kebutuhan Penagihan & Faktur Institusi
1. **Pembuatan Dokumen Faktur (Ekspor PDF)**
   * Pembuatan invoice berformat PDF resmi dengan kop surat, stempel digital, dan tanda tangan resmi DIFOSS Holding.
   * Rincian: Nomor Faktur, Tanggal, Nama Universitas/Instansi, NPWP, Rincian Paket/Layanan, Subtotal, PPN 11%, dan Total Akhir.
2. **Permintaan Penawaran & Pro-Forma Invoice**
   * Pengunduhan Pro-Forma Invoice sebelum pembayaran dilakukan guna pengajuan anggaran ke bagian keuangan rektorat/fakultas.
3. **Kuitansi Resmi & Faktur Pajak**
   * Pengunduhan tanda terima kuitansi lunas secara otomatis setelah pembayaran terverifikasi.
   * Tautan pengunduhan e-Faktur pajak setelah diterbitkan oleh tim keuangan DIFOSS.

## Kebutuhan Fungsional
* Integrasi SDK atau Webview Payment Gateway Indonesia (seperti Midtrans, Xendit, atau DOKU).
* Penampil dokumen invoice (PDF viewer) dalam aplikasi dengan kemampuan perbesaran (zoom), pembagian tautan, dan pengunduhan file.
* Sinkronisasi status bayar otomatis melalui webhook dan penarikan berkala (polling) untuk memperbarui status pesanan secara seketika.
