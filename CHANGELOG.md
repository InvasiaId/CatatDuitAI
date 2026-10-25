# Changelog

Semua perubahan dan pembaruan penting pada aplikasi **CatatDuit AI** akan didokumentasikan dalam berkas ini.

Format changelog mengacu pada [Keep a Changelog](https://keepachangelog.com/id/1.0.0/) dan menganut [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-10-25

### Ditambahkan (Added)
* **Omnichannel Mobile Experience**: Aplikasi Flutter Android mandiri terintegrasi penuh dengan Bot Telegram.
* **Branding & Identitas Baru**: Logo dan launcher icon resmi beresolusi tinggi di seluruh kepadatan layar Android (`mdpi` hingga `xxxhdpi`).
* **Sistem Autentikasi OTP Telegram**:
  * Penautan akun tanpa password melalui kode OTP 6-digit.
  * Masa kedaluwarsa OTP 5 menit (*cooldown protection*).
  * Perlindungan brute-force progressive exponential lockout dengan pesan waktu tunggu interaktif.
  * Sesi login persisten (*auto-login*) menggunakan token terenkripsi.
* **Pencatatan Transaksi Cerdas**:
  * Input nominal dengan pemformatan otomatis ribuan, ratusan ribu, dan jutaan rupiah.
  * Tombol jalan pintas nominal cepat (`+10rb`, `+50rb`, `+100rb`, `+500rb`, `+1jt`).
  * Dukungan multi-dompet (*Cash*, *Bank Transfer*, *E-Wallet*).
* **Asisten Keuangan FinTech Cerdas (AI)**:
  * Konsultasi interaktif seputar saldo, ringkasan, dan strategi tabungan.
  * Fitur pesan suara (*Voice Note*) untuk konsultasi hands-free.
  * Fitur OCR kamera struk (*AI Vision*) dengan filter validasi dokumen belanja asli.
  * Pelindung keamanan prompt injection dan sensor arsitektur teknis internal.
* **Analisis & Kuota Anggaran (*Budgeting*)**:
  * Diagram batang visual interaktif (Mingguan, Bulanan, Tahunan).
  * Progress kuota anggaran dengan badge indikator (*Aman*, *Mendekati Batas*, *Melebihi Kuota*).
  * Rekomendasi tips hemat pintar (*Smart Financial Tips*).
* **Ekspor Laporan Resmi**: Fitur unduh dan bagikan rekap transaksi format Microsoft Excel (`.xlsx`).
* **Kepatuhan Izin Android**: Permintaan izin dinamis saat dibutuhkan (*runtime permissions*) untuk Kamera, Mikrofon, dan Notifikasi.

### Keamanan (Security)
* Enkripsi sesi mobile berbasis timing-safe HMAC SHA-256.
* Rate limiting ketat per IP dan per User ID.
* Sanitasi input mendalam pada chatbot AI untuk mencegah prompt injection.
