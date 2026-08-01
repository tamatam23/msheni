# 📋 Administrasi Guru - Kompikids WebApp

Sistem Informasi Akademik Terpadu berbasis **Google Apps Script (GAS)** yang dirancang khusus untuk efisiensi administrasi guru di lingkungan sekolah Indonesia.

## 🚀 Deskripsi Proyek
Administrasi Guru adalah solusi *web-app* berbasis *spreadsheet* yang memungkinkan guru mengelola administrasi kelas dengan antarmuka modern, responsif, dan terintegrasi secara *real-time*.

## 🛠 Teknologi Utama
*   **Backend**: Google Apps Script (GAS)
*   **Frontend**: HTML5, Tailwind CSS
*   **Database**: Google Sheets
*   **Library Tambahan**: SheetJS (XLSX) untuk manajemen data Excel.

## 📋 Fitur Utama
1.  **Dashboard Statistik**: Pemantauan jumlah siswa (L/P), statistik kehadiran *real-time*, daftar ulang tahun bulan berjalan, dan agenda akademik.
2.  **Manajemen Siswa (CRUD)**: Input data siswa, unggah massal melalui file Excel (.xlsx), dan dukungan penyimpanan foto berbasis Base64.
3.  **Rutinitas Harian**:
    *   **Absensi Massal**: Sistem absensi harian yang terintegrasi lintas kelas.
    *   **Jurnal Mengajar**: Log aktivitas mengajar dengan fitur ekspor PDF.
    *   **Catatan Siswa**: Pencatatan perkembangan akademik dan insidental (kejadian).
4.  **Manajemen Waktu**: Jadwal mengajar mingguan dan sistem kalender akademik interaktif.
5.  **Evaluasi Akademik**: Sistem penilaian (teori/praktik) dengan konversi predikat otomatis dan dukungan impor/ekspor nilai Excel.
6.  **Sistem**: Pengaturan profil sekolah, identitas guru, dan manajemen akses akun yang aman.

## 🏗 Struktur Arsitektur
*   **`Code.gs`**: Berfungsi sebagai *server-side controller* yang menangani koneksi ke Google Sheets (Database) dan *routing* web aplikasi.
*   **`Index.html`**: Antarmuka pengguna (UI) yang dibangun menggunakan Tailwind CSS untuk estetika modern dan responsivitas mobile.
*   **JavaScript (Embedded)**: Menangani logika sisi klien, sinkronisasi data antar modul, dan manipulasi DOM untuk pengalaman pengguna yang dinamis.

## ⚙️ Petunjuk Setup (Google Apps Script)
1.  Buat Google Sheet baru dan siapkan sheet dengan nama: `DataSiswa`, `Absensi`, `JurnalMengajar`, `CatatanSiswa`, `Penilaian`, `JadwalMengajar`, `KalenderAkademik`, `MasterData`, `MasterPredikat`, dan `PengaturanProfil`.
2.  Buka **Extensions > Apps Script** di Google Sheet tersebut.
3.  Salin kode backend ke `Code.gs`.
4.  Buat file HTML baru bernama `Index.html` dan salin kode frontend ke sana.
5.  Tekan **Deploy > New Deployment**, pilih **Web App**, set *Execute as* ke **Me**, dan *Who has access* ke **Anyone**.
6.  Gunakan URL yang dihasilkan untuk mengakses aplikasi.

## 👤 Penulis
*   **KompiApps** - Pengembang utama sistem.

---
*Dikembangkan dengan semangat kemudahan administrasi pendidikan Indonesia.*
