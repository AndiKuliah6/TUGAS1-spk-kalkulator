# SPK Calculator

SPK Calculator adalah kakulator interaktif berbasis web yang dibangun dengan HTML, CSS, dan Vanilla JavaScript murni untuk mensimulasikan perhitungan tiga metode Sistem Pendukung Keputusan (SPK):
- **SAW** (Simple Additive Weighting)
- **Fuzzy Tsukamoto**
- **AHP** (Analytic Hierarchy Process)

Aplikasi ini berjalan sepenuhnya di sisi klien (browser lokal) tanpa memerlukan bahasa pemrograman server (backend) atau database.

## 🚀 Fitur Unggulan

- **Antarmuka Interaktif:** Desain antarmuka (SPA/Single Page Application) dengan sistem tab untuk berpindah metode secara instan.
- **Responsif:** Tampilan desain fleksibel yang menyesuaikan dengan baik di perangkat desktop maupun seluler.
- **Perhitungan Transparan:** Tidak hanya menampilkan hasil pemenang di akhir, tetapi juga menjabarkan urutan langkah-langkah perhitungan matematika secara rinci (step-by-step) sehingga sangat cocok untuk alat pembelajaran.
- **Studi Kasus Default:** Dilengkapi dengan nilai *default* (bawaan) berdasarkan contoh studi kasus (misalnya, Manajemen Katering "Lansia Sehat") sehingga aplikasi dapat langsung diuji coba.

## 🛠️ Cara Menggunakan (Panduan Pengguna)

1. **Buka Aplikasi:** Klik ganda (*double-click*) pada file `spk-calculator.html` untuk membukanya secara langsung menggunakan peramban web (seperti Google Chrome, Firefox, Safari, atau Microsoft Edge).
2. **Navigasi Metode:** Gunakan menu tabulasi di bagian atas halaman untuk memilih metode SPK (SAW, Fuzzy Tsukamoto, atau AHP) yang ingin Anda hitung.
3. **Konfigurasi Variabel:** 
   - Anda bebas menambah/mengurangi jumlah alternatif, jumlah kriteria, maupun mengubah nilai batasan kurva pada Fuzzy Tsukamoto.
4. **Input Angka:** Masukkan nilai matriks ke dalam kotak yang tersedia atau geser tombol *slider* untuk simulasi cepat.
5. **Jalankan Perhitungan:** Tekan tombol **"Hitung"** pada bagian bawah. Aplikasi akan secara otomatis menurunkan (scroll) ke bagian bawah halaman yang menampilkan penjabaran rumus dan hasil perankingan atau keputusan akhirnya.
6. **Reset:** Tekan tombol **"Reset"** untuk mengembalikan seluruh angka parameter ke posisi bawaan (default).

## 📂 Struktur Berkas

Proyek ini dibuat menggunakan pendekatan *single-file* agar portabel dan mudah dibagikan.
- `spk-calculator.html`: Memuat struktur HTML (elemen antarmuka), style CSS (desain warna & tata letak), dan skrip logika matematika berbasis JavaScript.

## 📚 Manfaat 

Alat (*tools*) ini direkomendasikan penggunaannya oleh mahasiswa, pengajar (dosen), dan pengambil keputusan profesional yang ingin memvalidasi hasil uji hitungan manual terhadap metode AHP, SAW, maupun Logika Fuzzy mereka dengan cepat.
