# Feature Specification: Digital Asset Vault & License Management

## Status
* **Sumber Asal**: Fitur Baru (Mobile-First / Belum ada di website saat ini)
* **Prioritas**: Menengah / P1

## Latar Belakang & Kebutuhan
DIFOSS menjual produk digital seperti paket tema dan plugin untuk SLiMS, EPrints, dan OJS. Saat ini distribusinya masih dilakukan secara manual. Fitur Digital Asset Vault memungkinkan pembeli terverifikasi mengakses paket zip perangkat lunak, kunci lisensi aktif, serta dokumentasi panduan pemasangan langsung dari aplikasi.

## Kebutuhan Fungsional
1. **Daftar Produk yang Dimiliki**
   * Tab khusus berisi daftar tema, plugin, dan paket starter yang berhasil dibeli pengguna.
   * Rincian: Nama Produk, Tanggal Pembelian, Nomor Kunci Lisensi, dan Nomor Versi Terakhir.
2. **Manajemen Kunci Lisensi**
   * Tombol satu sentuhan untuk menyalin (copy) kunci lisensi.
   * Menampilkan domain terdaftar yang terikat pada lisensi (contoh: `jurnal.kampus.ac.id`).
   * Formulir pengajuan perubahan tautan domain jika instansi melakukan relokasi alamat server.
3. **Pengunduhan Berkas & Dokumentasi**
   * Unduh paket berkas zip atau kirim tautan unduhan langsung ke email institusi yang terdaftar.
   * Penampil panduan instalasi (README dan buku panduan setup) langsung di dalam aplikasi.
4. **Pemberitahuan Pembaruan Versi**
   * Notifikasi otomatis jika tersedia versi baru atau tambalan keamanan pada tema/starter kit yang dimiliki (misal: penyesuaian kompatibilitas untuk rilis OJS versi terbaru).
