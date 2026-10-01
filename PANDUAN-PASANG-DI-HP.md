# Memasang Aplikasi di HP (PWA)

Aplikasi hanya bisa dipasang bila dibuka lewat alamat **https://**.
File yang dibuka dari folder Unduhan (alamat content:// atau file://) tidak bisa dipasang.

## 1. Unggah ke GitHub Pages (gratis)
1. Buat akun di github.com, lalu buat repository baru (mis. `monitoring-dokumen`), pilih Public.
2. Klik "Add file > Upload files", unggah SEMUA isi folder ini
   (index.html, manifest.webmanifest, sw.js, dan folder icons), lalu Commit.
3. Buka Settings > Pages. Pada "Branch" pilih `main` dan folder `/ (root)`, lalu Save.
4. Tunggu 1-2 menit. Alamatnya: https://NAMAAKUN.github.io/monitoring-dokumen/

## 2. Pasang di HP
- Android (Chrome): buka alamat di atas. Ketuk "Pasang aplikasi" di menu samping,
  atau menu titik tiga > "Instal aplikasi".
- iPhone (Safari): buka alamat di atas, ketuk Bagikan > "Tambah ke Layar Utama".

Ikon "Monitoring Dokumen" akan muncul di layar utama dan terbuka layar penuh seperti aplikasi biasa.

## 3. Google Drive
Alamat GitHub Pages yang sama (https://NAMAAKUN.github.io, tanpa nama repository)
dimasukkan ke "Authorized JavaScript origins" di Google Cloud Console.

## Memperbarui aplikasi
Ganti file index.html di repository. Bila tampilan lama masih muncul, ubah angka versi
pada `CACHE` di sw.js (mis. monitoring-dokumen-v2), lalu tutup dan buka ulang aplikasi.

## Catatan
- Aplikasi bisa dibuka tanpa internet setelah pernah dibuka sekali, tetapi memuat file Excel
  dari Drive, login Google, dan sinkronisasi tetap butuh internet.
- Data Excel tidak disimpan permanen di HP. Buka ulang file Excel setiap kali aplikasi dibuka.
