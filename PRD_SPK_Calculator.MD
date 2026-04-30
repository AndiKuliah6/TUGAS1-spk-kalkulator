# PRD: SPK Calculator (SAW, Fuzzy Tsukamoto, AHP)

## 1. Overview
SPK Calculator adalah aplikasi web berbasis Single-Page Application (SPA) yang menyediakan alat bantu perhitungan interaktif untuk tiga metode Sistem Pendukung Keputusan (SPK) yang berbeda:
1. Simple Additive Weighting (SAW)
2. Fuzzy Tsukamoto
3. Analytic Hierarchy Process (AHP)

## 2. Fitur Utama

### 2.1 Tab Navigasi Terpadu
- Menggunakan menu tab untuk berpindah antar metode (SAW, Fuzzy, AHP) tanpa memuat ulang halaman.

### 2.2 Modul 1: SAW (Simple Additive Weighting)
- **Studi Kasus:** Pemilihan Supplier Katering "Lansia Sehat".
- **Konfigurasi Dinamis:** Pengguna dapat menentukan jumlah alternatif (2-10) dan kriteria (1-8).
- **Penyesuaian Kriteria:** Memungkinkan pengaturan nama kriteria, jenis (Cost/Benefit), dan bobot secara real-time.
- **Validasi Bobot:** Memberikan indikator peringatan jika total bobot tidak sama dengan 1.0.
- **Matriks Keputusan:** Tabel input dinamis untuk nilai alternatif terhadap setiap kriteria.
- **Hasil Perhitungan:** Menampilkan langkah-langkah detail, mulai dari normalisasi matriks, perhitungan preferensi (V), hingga perankingan akhir dan penentuan rekomendasi terbaik.

### 2.3 Modul 2: Fuzzy Inference System (Tsukamoto)
- **Studi Kasus:** Penentuan Stok Harian Nasi Katering "Lansia Sehat".
- **Parameter Fungsi Keanggotaan:** Input parameter untuk kurva linear turun/naik untuk variabel "Sisa Stok" dan "Jumlah Pesanan".
- **Input Nilai Crisp:** Menggunakan slider (range) dan text input tersinkronisasi untuk memasukkan nilai aktual.
- **Visualisasi Hasil:** Menampilkan proses fuzzifikasi dengan bar persentase (μ), evaluasi rule base, invers fungsi output, dan nilai akhir defuzzifikasi (weighted average) beserta interpretasi keputusannya.

### 2.4 Modul 3: AHP (Analytic Hierarchy Process)
- **Studi Kasus:** Pemilihan Lokasi Kantor PT. NusaTech Inovasi.
- **Matriks Dinamis:** Memungkinkan pengguna memasukkan nama kriteria dan alternatif, lalu men-generate matriks perbandingan berpasangan.
- **Perhitungan Otomatis:** Menghitung resiprokal secara otomatis (jika C1 thd C2 = 3, maka C2 thd C1 = 1/3).
- **Uji Konsistensi:** Menampilkan nilai Lambda Max (λmax), Consistency Index (CI), dan mengevaluasi validitas melalui Consistency Ratio (CR).
- **Sintesis Akhir:** Mengalikan bobot kriteria dengan bobot alternatif untuk menghasilkan skor global dan memunculkan rekomendasi pemenang.

## 3. Spesifikasi UI/UX & Desain
- **Warna & Tema:** Menggunakan perpaduan warna Navy (`#0d2845`), Biru (`#1565c0`), Teal (`#00897b`), dan Hijau terang untuk notifikasi sukses, memberikan kesan aplikasi kalkulator yang profesional dan analitis.
- **Tipografi:** Menggunakan font Outfit (untuk Heading), DM Sans (untuk Body), dan JetBrains Mono (untuk Angka/Rumus matematis).
- **Responsivitas:** Desain grid fleksibel dan tabel yang bisa di-*scroll* (overflow) agar tetap proporsional untuk diakses pada layar mobile dan desktop.
- **Interaksi Animasi:** Menampilkan interaksi animasi *fade-up* secara halus saat memunculkan hasil perhitungan.

## 4. Teknologi yang Digunakan
- **HTML5:** Struktur semantik aplikasi SPA.
- **CSS3:** Styling menggunakan Flexbox, Grid, CSS Variables, dan native transitions.
- **Vanilla JavaScript (ES6):** Mengendalikan manipulasi DOM untuk UI yang dinamis, serta menjalankan seluruh logika matematika kompleks tanpa bergantung pada library eksternal (murni browser).
