# 🌸 WIBU-TERMINAL - Pterodactyl Bypass 🌸

![Version](https://img.shields.io/badge/Version-1.0_TokyoNight-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Pterodactyl-brightgreen.svg)
![NodeJS](https://img.shields.io/badge/Node-v18+-orange.svg)

WIBU-TERMINAL adalah *script bypass* ajaib yang menyulap panel Pterodactyl Anda yang tadinya terkekang, menjadi **Terminal Linux Penuh (Full Root Access-like) secara Online!**

Dengan menggunakan *theme* **Tokyo Night Hacker Anime**, terminal online ini sangat memanjakan mata dan memberikan Anda kebebasan untuk menginstal banyak bot sekaligus, menjalankan PM2, mengunduh file, atau sekadar melakukan *flexing* terminal Linux di browser Anda layaknya **Termux versi Web**.

## 🚀 Fitur Unggulan

*   **🔓 Bypass Pterodactyl:** Menembus batas *port* Pterodactyl menggunakan terowongan canggih (Cloudflared Tunnel).
*   **💻 Full Shell Access:** Bebas mengeksekusi perintah Linux (`apt`, `npm`, `pm2`, `wget`, `curl`, dll) persis seperti VPS pribadi.
*   **🌸 Anime / Tokyo Night Theme:** Tampilan konsol yang sangat estetik dengan warna neon pastel yang tidak membuat mata sakit.
*   **⚡ 1-Click Install:** Sangat mudah dipasang, bot otomatis mengunduh komponen mesin (`ttyd` & `cloudflared`) dengan sendirinya tanpa ribet.

---

## 🛠️ Cara Memasang di Panel Pterodactyl

1.  **Download Repo:** Klik tombol hijau `Code` di atas, lalu pilih **Download ZIP**.
2.  **Upload ke Pterodactyl:** Buka panel Pterodactyl Anda, pastikan Anda berada di direktori paling depan (`/home/container/` atau `/`). Jika ada file lama, disarankan dihapus terlebih dahulu.
3.  **Ekstrak (Unarchive):** Upload file ZIP tadi dan klik *Unarchive*.
4.  **Keluarkan File:** Pindahkan (`Move`) file `index.js` dan `package.json` dari dalam folder agar berada tepat di halaman utama (`/`).
5.  **Jalankan (START):** Buka menu **Console** lalu klik tombol **START**.
6.  **Tunggu & Akses:** Mesin akan mengunduh komponen selama 10-20 detik. Setelah selesai, terminal akan mencetak link khusus (contoh: `https://xxxx.trycloudflare.com`).
7.  **Selesai!** Klik / Buka link tersebut di browser HP atau Laptop Anda. Terminal Hacker Anime siap digunakan!

---

## 💡 Tips & Trik Penggunaan

*   **Menjalankan Bot WA:** Setelah masuk ke Terminal Web, Anda bisa meng-*clone* script bot Anda dan menyalakannya menggunakan PM2, jadi bot akan terus berjalan di latar belakang!
*   **Batas Waktu Link:** Link dari Cloudflare ini bersifat dinamis (sementara). Jika panel Pterodactyl di-restart, link URL-nya akan berubah menjadi yang baru.

> *© 2026 - Dioptimalkan eksklusif untuk WibuVpnStore*

---

## 🛠️ Panduan Mengatasi Masalah (Troubleshooting)

**1. Muncul Error `EACCES` atau "Permission Denied"**
*   **Penyebab:** Biasanya terjadi jika file `ttyd` atau `cloudflared` yang didownload rusak/kosong karena gangguan jaringan.
*   **Solusi:** Buka tab **Files** di Pterodactyl, **HAPUS** file bernama `ttyd` dan `cloudflared` (jika ada), lalu klik **Start** lagi agar script mendownload ulang file yang utuh.

**2. Terminal tertutup langsung setelah dibuka**
*   **Penyebab:** Mesin Pterodactyl Anda mungkin tidak mendukung `bash`.
*   **Solusi:** Script versi terbaru (V1.1) sudah kami *update* dengan sistem Fallback Anti-Alergi. Pastikan Anda sudah mengunduh file `index.js` versi yang paling baru dari Github ini!
