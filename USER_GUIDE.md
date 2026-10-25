# 📘 Panduan Pengguna CatatDuit AI (User Guide)

Selamat datang di **CatatDuit AI**! Panduan ini dirancang untuk membantu Anda memahami, menginstal, dan memanfaatkan seluruh fitur cerdas pengelolaan keuangan personal secara optimal melalui aplikasi Android dan bot Telegram.

---

## 📑 Daftar Isi
1. [Persyaratan & Instalasi APK](#1-persyaratan--instalasi-apk)
2. [Tautkan Akun & Login OTP Telegram](#2-tautkan-akun--login-otp-telegram)
3. [Mengenal Antarmuka Utama (Dashboard)](#3-mengenal-antarmuka-utama-dashboard)
4. [Mencatat Transaksi Finansial](#4-mencatat-transaksi-finansial)
5. [Fitur Cerdas AI: Scan Struk & Pesan Suara](#5-fitur-cerdas-ai-scan-struk--pesan-suara)
6. [Analisis Pengeluaran & Kuota Anggaran](#6-analisis-pengeluaran--kuota-anggaran)
7. [Konsultasi Finansial Bersama AI Assistant](#7-konsultasi-finansial-bersama-ai-assistant)
8. [Unduh Laporan Keuangan Excel (.xlsx)](#8-unduh-laporan-keuangan-excel-xlsx)
9. [Manajemen Izin Perangkat](#9-manajemen-izin-perangkat)
10. [Pertanyaan Umum (FAQ) & Solusi Masalah](#10-pertanyaan-umum-faq--solusi-masalah)

---

## 1. Persyaratan & Instalasi APK

### Kebutuhan Minimum Perangkat:
* **Sistem Operasi**: Android 6.0 (Marshmallow / API 23) atau versi yang lebih tinggi.
* **Koneksi Jaringan**: Internet aktif (Wi-Fi atau Data Seluler).
* **Aplikasi Telegram**: Terinstal di ponsel atau dapat diakses via web.

### Langkah-langkah Pemasangan (Sideloading):
1. **Unduh File APK**: Unduh berkas installer `CatatDuitAi.apk` dari rilis resmi di GitHub.
2. **Izinkan Instalasi dari Sumber Tak Dikenal**:
   * Buka file yang baru diunduh.
   * Jika muncul peringatan keamanan sistem Android, pilih **Pengaturan / Settings**.
   * Aktifkan centang **"Izinkan dari sumber ini"** (*Allow from this source*).
3. **Selesaikan Instalasi**: Ketuk **Instal**, lalu tunggu hingga proses pemasangan selesai.
4. **Verifikasi Keamanan (Opsional)**: Anda dapat mencocokkan nilai hash SHA-256 berkas dengan file `SHA256SUMS.txt` untuk memastikan keaslian paket biner.

---

## 2. Tautkan Akun & Login OTP Telegram

Aplikasi CatatDuit AI menggunakan sistem penautan akun berbasis OTP (*One-Time Password*) yang aman dan terintegrasi langsung dengan akun Telegram Anda tanpa perlu mengingat kata sandi.

```
+------------------+         Perintah /link          +-------------------+
|  Bot Telegram    |  ===========================>   | Dapatkan 6-Digit  |
|  @CatatDuitBot   |                                 | Kode OTP (5 mnt)  |
+------------------+                                 +-------------------+
         |                                                     |
         v                                                     v
+------------------+      Verifikasi & Hubungkan     +-------------------+
| Akun Terhubung!  |  <===========================   | Masukkan di App   |
| Sesi Tersimpan   |                                 | Android           |
+------------------+                                 +-------------------+
```

### Langkah Login:
1. Buka aplikasi **CatatDuit AI** di ponsel Anda.
2. Di layar Onboarding, ketuk tombol **"Tautkan Akun Telegram"** atau **"Get Started"**.
3. Buka bot Telegram CatatDuit Anda, lalu kirim perintah:
   ```
   /link
   ```
   *(atau cukup ketik `/kode`)*
4. Bot akan membalas dengan **6-digit kode angka** yang berlaku selama **5 menit**.
5. Masukkan 6 angka tersebut ke dalam aplikasi Android.
6. Ketuk tombol **"Verifikasi & Hubungkan"**.
7. Aplikasi akan langsung memuat data portofolio Anda. Sesi login akan disimpan secara persisten, sehingga Anda tidak perlu memasukkan kode lagi saat membuka aplikasi berikutnya.

> [!NOTE]
> Demi keamanan, kode OTP hanya bisa dibuat sekali setiap 5 menit. Jika Anda salah memasukkan kode beberapa kali berturut-turut, sistem proteksi bertingkat (*progressive lockout*) akan mengunci permintaan sementara waktu.

---

## 3. Mengenal Antarmuka Utama (Dashboard)

Setelah berhasil masuk, Anda akan disambut di halaman **Beranda**:
* **Kartu Saldo Utama (*Total Balance*)**: Menampilkan akumulasi kekayaan bersih dari seluruh dompet dan rekening Anda. Terdapat tombol ikon mata untuk menyembunyikan atau menampilkan nominal saldo.
* **Ringkasan Arus Kas Bulan Ini**: Indikator persentase pemasukan vs pengeluaran bulan berjalan.
* **Aksi Cepat (*Quick Action Chips*)**:
  * **+ Pemasukan**: Mencatat pemasukan baru secara instan.
  * **- Pengeluaran**: Mencatat pengeluaran harian.
  * **Scan Struk**: Membuka kamera pintar untuk memindai nota fisik.
  * **Tanya AI**: Berpindah langsung ke ruang konsultasi cerdas.
* **Daftar Transaksi Terbaru**: Menampilkan catatan belanja terakhir dengan kategori, dompet sumber, dan tombol hapus cepat jika ada kesalahan input.

---

## 4. Mencatat Transaksi Finansial

Anda dapat mencatat transaksi secara manual dengan mudah:

1. Ketuk tombol **(+) Melayang** (*Floating Action Button*) di sudut kanan bawah layar, atau pilih tombol **Pemasukan / Pengeluaran** di beranda.
2. Pilih tipe transaksi: **🔴 Keluar** atau **🟢 Masuk**.
3. **Ketik Nominal**: Gunakan shortcut tombol cepat (`+10rb`, `+50rb`, `+100rb`, `+500rb`, `+1jt`) untuk pengisian super cepat. Nominal otomatis berformat ribuan, ratusan ribu, dan jutaan rupiah secara rapi.
4. Tulis **Keterangan / Nama Toko** (contoh: *Kopi Kenangan*, *Beli Bensin*, *Gaji Bulanan*).
5. Pilih **Kategori** yang sesuai (*Makanan & Minuman, Transportasi, Belanja, Tagihan, Hiburan, dll*).
6. Tentukan **Dompet / Rekening** sumber dana (*Tunai, Bank BCA, Mandiri, GoPay, OVO, ShopeePay*).
7. Ketuk **"Simpan Transaksi"**. Data akan langsung tersinkronisasi ke bot Telegram secara realtime.

---

## 5. Fitur Cerdas AI: Scan Struk & Pesan Suara

### 📷 Pindai Struk Belanja Fisik (AI Vision OCR)
1. Pada menu Beranda, ketuk **"Scan Struk"**.
2. Izinkan akses kamera saat aplikasi meminta izin untuk pertama kali.
3. Arahkan kamera ke struk belanja kertas (pastikan pencahayaan cukup dan teks total belanja terbaca jelas).
4. Tekan tombol bidik foto.
5. Asisten AI akan memproses gambar, membaca nama merchant, rincian belanja, serta total nominal secara otomatis.
6. Anda cukup memeriksa hasilnya lalu mengonfirmasi penyimpanan.
*(Catatan: Sistem dilengkapi filter pencegah deteksi palsu jika foto yang diambil bukan merupakan struk belanja).*

### 🎙️ Kirim Catatan Suara (AI Voice Note)
1. Masuk ke tab **"Tanya AI"**.
2. Ketuk tombol **"Kirim Pesan Suara (Voice Note)"** atau ikon mikrofon.
3. Izinkan akses mikrofon saat diminta.
4. Ucapkan transaksi Anda secara santai, contoh:
   > *"Tadi siang makan bakso bareng teman habis 35 ribu bayar pakai GoPay"*
5. Sistem AI akan mengekstrak nominal, dompet, dan kategori secara cerdas, lalu mengonfirmasikannya kepada Anda.

---

## 6. Analisis Pengeluaran & Kuota Anggaran

Buka tab **Analisis** (ikon grafik batang) di bilah navigasi bawah:
* **Grafik Tren Pengeluaran**: Menampilkan diagram batang historis pengeluaran Anda. Anda dapat beralih antara filter **Minggu**, **Bulan**, dan **Tahun**.
* **Ketuk Batang Diagram**: Ketuk salah satu batang untuk melihat detail pengeluaran pada periode tersebut.
* **Kategori Pengeluaran Terbesar**: Menampilkan diagram persentase donat dan daftar kategori dengan porsi pengeluaran paling dominan.
* **Batas Kuota Anggaran (*Budgeting*)**:
  * Tentukan limit maksimal pengeluaran per kategori.
  * Sistem memberikan badge warna indikator: **🟢 Aman**, **🟡 Mendekati Batas (>= 80%)**, dan **🔴 Melebihi Kuota**.
* **Smart Financial Tips**: AI menganalisis kebiasaan belanja Anda dan memberikan tips proaktif untuk menghemat pengeluaran yang tidak perlu.

---

## 7. Konsultasi Finansial Bersama AI Assistant

Buka tab **Tanya AI** untuk berkonsultasi seputar kesehatan keuangan Anda:
* **Tombol Saran Cepat**: Tersedia tombol pintas seperti `/saldo`, `/riwayat`, `/anggaran`, `/target`, dan `/bantuan`.
* **Tanya Bebas dalam Bahasa Alami**: Anda bisa menanyakan hal-hal seperti:
  * *"Berapa total pengeluaran kopi saya bulan ini?"*
  * *"Apakah keuangan saya bulan ini defisit?"*
  * *"Berikan rekomendasi cara menabung 5 juta dalam 3 bulan"*
* **Perlindungan Privasi AI**: AI dikonfigurasi secara ketat hanya untuk konsultasi finansial personal dan menolak instruksi di luar topik maupun manipulasi data teknis.

---

## 8. Unduh Laporan Keuangan Excel (.xlsx)

Anda dapat mengunduh rekap riwayat keuangan dalam format spreadsheet resmi Microsoft Excel:
1. Masuk ke tab **Transaksi** atau tab **Dompet**.
2. Ketuk ikon / tombol **"Unduh Laporan Excel (.xlsx)"** di pojok kanan atas.
3. Sistem akan memproses dan mengompilasi seluruh transaksi Anda menjadi lembar kerja Excel yang rapi dengan kolom Tanggal, Jenis, Kategori, Nominal, Dompet, dan Catatan.
4. Setelah muncul notifikasi **"Laporan Excel Siap!"**, Anda dapat langsung:
   * **Buka File**: Membuka berkas menggunakan Microsoft Excel, Google Sheets, atau WPS Office.
   * **Bagikan**: Mengirim berkas laporan via WhatsApp, Telegram, Email, atau menyimpannya ke Google Drive.

---

## 9. Manajemen Izin Perangkat

Untuk memberikan pengalaman terbaik, aplikasi memerlukan beberapa izin fungsional Android:

| Izin Perangkat | Fungsi & Kegunaan | Waktu Permintaan |
| :--- | :--- | :--- |
| **Kamera (`CAMERA`)** | Mengambil foto struk belanja untuk diproses oleh OCR AI. | Saat pertama kali mengetuk tombol *Scan Struk*. |
| **Mikrofon (`RECORD_AUDIO`)** | Merekam suara Anda saat menggunakan fitur *Voice Note* di chat AI. | Saat pertama kali mengetuk tombol *Voice Note*. |
| **Notifikasi (`POST_NOTIFICATIONS`)** | Memberi tahu pengingat catat harian dan notifikasi batas anggaran. | Saat pertama kali masuk ke menu utama. |

> [!NOTE]
> Anda dapat mengubah atau mencabut izin ini kapan saja melalui menu **Pengaturan Ponsel > Aplikasi > CatatDuit AI > Izin**.

---

## 10. Pertanyaan Umum (FAQ) & Solusi Masalah

#### Q: Mengapa bot Telegram tidak mengirimkan kode OTP?
* Pastikan Anda telah memulai percakapan dengan bot dengan mengetik `/start` terlebih dahulu.
* Pastikan koneksi internet ponsel stabil.
* Jika sudah meminta kode kurang dari 5 menit yang lalu, gunakan kode sebelumnya atau tunggu hingga countdown 5 menit selesai.

#### Q: Apakah data keuangan saya aman jika ponsel hilang?
* Ya. Aplikasi tidak menyimpan kata sandi plain-text. Akses aplikasi diamankan dengan token sesi terenkripsi. Anda dapat memutus sesi penautan perangkat kapan saja langsung melalui bot Telegram dengan perintah `/logout` atau `/revokesessions`.

#### Q: Kenapa foto meja atau benda acak ditolak oleh AI Vision?
* Asisten AI telah dilengkapi model validasi cerdas untuk memastikan hanya dokumen struk atau nota pembayaran sah yang dicatat ke sistem pembukuan Anda.

#### Q: Bagaimana cara logout dari aplikasi?
* Buka tab **Dompet / Profil**, gulir ke bawah, lalu ketuk tombol **Logout**. Token sesi di ponsel akan dibersihkan secara aman.
