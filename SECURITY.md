# Kebijakan Keamanan (Security Policy)

Keamanan data keuangan dan privasi pengguna adalah prioritas tertinggi dalam pengembangan **CatatDuit AI**.

---

## Versi yang Didukung

Pembaruan keamanan dan perbaikan celah secara aktif diberikan untuk versi berikut:

| Versi | Didukung |
| :--- | :--- |
| 1.0.x (Terbaru) | :white_check_mark: |
| < 1.0.0 | :x: |

---

## Fitur & Arsitektur Keamanan Bawaan
* **HMAC Timing-Safe Verification**: Verifikasi OTP bebas dari eksploitasi timing-attack.
* **Progressive Rate Limiting**: Proteksi anti brute-force otomatis dengan peningkatan waktu lockout bertingkat.
* **Sensitive Architecture Shielding**: Asisten AI dan response metadata disensor secara otomatis agar tidak membocorkan detail infrastruktur internal, konfigurasi database, atau credential server.
* **Prompt Injection Defense**: Filter multi-lapis untuk memvalidasi dan menolak prompt berbahaya, perintah jailbreak, maupun injeksi skrip.

---

## Melaporkan Celah Keamanan (*Reporting a Vulnerability*)
Jika Anda menemukan kerentanan atau celah keamanan:
1. **Jangan mempublikasikan masalah tersebut secara terbuka** di GitHub Issues atau media publik.
2. Silakan laporkan detail temuan melalui tab **Security > Report a vulnerability** pada repositori GitHub ini.
3. Sertakan langkah-langkah reproduksi masalah (*Proof of Concept*).
4. Tim kami akan merespons dalam waktu 1x24 jam dan menyiapkan patch mitigasi sebelum informasi celah dipublikasikan.
