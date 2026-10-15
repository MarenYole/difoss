# Feature Specification: Mobile Security & Biometric Authentication

## Status
* **Sumber Asal**: Fitur Baru (Mobile-First / Belum ada di website saat ini)
* **Prioritas**: Utama / P0

## Latar Belakang & Kebutuhan
Mengingat aplikasi ini digunakan oleh pengelola institusi untuk mengakses data transaksi, kredensial konfigurasi, serta kunci lisensi perangkat lunak, standar keamanan tingkat tinggi pada platform mobile merupakan hal mutlak.

## Kebutuhan Fungsional
1. **Autentikasi Biometrik**
   * Dukungan sidik jari (Touch ID / Android BiometricPrompt) dan pengenalan wajah (Face ID / Android Face Unlock).
   * Opsi cadangan berupa PIN perangkat atau kata sandi akun DIFOSS jika biometrik gagal.
   * Opsi di Pengaturan: "Aktifkan Masuk dengan Biometrik".
2. **Penyimpanan Token Terenkripsi**
   * Data sesi sensitif (JWT token, kunci rahasia) disimpan dalam modul keamanan perangkat keras (hardware-backed keystore):
     * iOS: Layanan Keychain (`kSecAttrAccessibleAfterFirstUnlock`).
     * Android: Android Keystore system dengan EncryptedSharedPreferences (enkripsi AES-256-GCM).
3. **Integritas Aplikasi & Proteksi Tingkat Lanjut**
   * Peringatan deteksi perangkat yang telah di-root atau jailbreak.
   * Penguncian otomatis aplikasi jika berada di latar belakang (background) selama lebih dari 5 menit.
   * Penerapan SSL Pinning untuk memblokir serangan penyadapan man-in-the-middle (MITM) pada komunikasi data antara aplikasi dan server DIFOSS.
   * Pengaburan kode (obfuscation) pada rilis produksi (R8/ProGuard pada Android, penanggalan simbol debug pada iOS).
