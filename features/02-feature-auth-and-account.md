# Feature Specification: Authentication & User Account Management

## Status
* **Sumber Asal**: Kesetaraan langsung dengan portal web ([/auth/login](https://holding.setiadifoss.org/auth/login))
* **Prioritas**: Utama / P0

## Ringkasan Fitur
Menyediakan identifikasi pengguna yang aman, manajemen sesi, serta profil instansi di seluruh aplikasi mobile.

## Kebutuhan Pengguna (User Stories)
* Sebagai pengelola instansi/kampus, saya ingin masuk dengan akun saya agar dapat melihat riwayat layanan, tema yang telah dibeli, dan saluran bantuan teknis.
* Sebagai administrator TI, saya ingin sesi saya tersimpan dengan aman di smartphone agar tidak perlu mengetikkan ulang kata sandi setiap kali membuka aplikasi.

## Kebutuhan Fungsional
1. **Layar Masuk (Login)**
   * Kolom input: Username atau Email Institusi, Kata Sandi.
   * Opsi "Ingat Saya" dengan penyimpanan token terenkripsi.
   * Pengalih visibilitas kata sandi (`Tampilkan / Sembunyikan`).
   * Tombol "Lupa Kata Sandi" mandiri melalui pengiriman tautan ke email terdaftar.
2. **Layar Profil Akun**
   * Informasi akun: Nama Lengkap, Afiliasi Instansi/Universitas, Peran (contoh: Pengelola Jurnal, Pustakawan, Sysadmin), Email, Nomor Telepon/WhatsApp.
   * Pembaruan profil (nama dan nomor kontak).
   * Dialog ganti kata sandi (kata sandi lama, kata sandi baru, konfirmasi kata sandi).
3. **Keamanan & Manajemen Sesi**
   * Penyimpanan kredensial memanfaatkan proteksi perangkat keras OS (iOS Keychain dan Android Keystore/EncryptedSharedPreferences).
   * Rotasi access token dan refresh token berbasis JWT.
   * Alur keluar akun (Logout) yang membersihkan data sesi lokal secara menyeluruh.

## Panduan Desain UI/UX Mobile
* Tampilan kartu bersih yang selaras dengan palet warna DIFOSS.
* Penyesuaian tata letak otomatis saat papan ketik virtual (keyboard) muncul, dengan kemampuan menutup papan ketik saat pengguna menyentuh area luar.
* Validasi formulir secara langsung (inline) dengan pesan kesalahan yang jelas dan ramah pengguna.
