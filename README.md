# Laporan Pengerjaan Tugas Akhir: Website Portofolio dengan Git Workflow

Repository ini adalah penyerahan untuk Tugas Akhir mata kuliah Dasar Pemrograman Web. Proyek ini mendokumentasikan seluruh proses pembuatan website portofolio pribadi, dari inisialisasi proyek hingga publikasi, dengan menerapkan alur kerja Git (Git Workflow) yang sistematis.

---

## Alur Kerja & Langkah Pengerjaan

Berikut adalah dokumentasi langkah demi langkah dari proses pengerjaan proyek ini, sesuai dengan riwayat commit yang tercatat di Git.

### Fase 1: Inisialisasi dan Commit Bertahap

Proyek dimulai dengan inisialisasi repository Git lokal dan dilanjutkan dengan pembangunan website section per section. Setiap bagian yang selesai langsung di-commit untuk menciptakan riwayat perubahan yang logis.

1.  **Navigasi ke Direktori Proyek**
    Langkah pertama adalah membuka terminal dan masuk ke folder kerja proyek.
    ```bash
    cd d:/laragon/www/pemweb/portofolio-saya
    <img width="746" height="178" alt="Screenshot 2025-11-01 223952" src="https://github.com/user-attachments/assets/bfaacaf2-870c-40d3-a33a-e78b82116820" />

    ```
2.  **Inisialisasi Proyek**
    Repository Git lokal dibuat di dalam folder proyek.
    ```bash
    git init
    ```

3.  **Commit #1: Struktur Dasar**
    Membuat kerangka dasar HTML dan file CSS, termasuk pengaturan variabel warna, font global, dan reset CSS dasar.
    * **Pesan Commit:** `Inisialisasi proyek dengan struktur HTML & CSS dasar`

4.  **Commit #2: Header & Navigasi**
    Menambahkan bagian `<header>` yang berisi logo dan menu navigasi utama.
    * **Pesan Commit:** `Tambah section header dan navigasi`

5.  **Commit #3: Section 'About'**
    Membuat section "Tentang Saya" yang berisi perkenalan diri, foto, dan tombol ajakan (call-to-action).
    * **Pesan Commit:** `buat section 'Tentang Saya' (About)`

6.  **Commit #4: Section 'Skills'**
    Menambahkan section "Kompetensi" yang menampilkan daftar bahasa pemrograman dan tools yang dikuasai dalam format kartu.
    * **Pesan Commit:** `buat section 'Kompetensi' (Skills)`

7.  **Commit #5: Section 'Projects'**
    Membuat section "Proyek Unggulan" untuk menampilkan portofolio proyek yang pernah dikerjakan.
    * **Pesan Commit:** `buat section 'Proyek Unggulan' (Projects)`

8.  **Commit #6: Section 'Contact' & Footer**
    Menyelesaikan halaman dengan menambahkan formulir kontak dan `<footer>`.
    * **Pesan Commit:** `Tambah section 'Kontak' dan footer halaman`

### Fase 2: Eksperimen Styling dengan Branch

Untuk mencoba ide desain baru tanpa merusak kode utama yang sudah stabil, sebuah branch baru dibuat.

1.  **Membuat Branch Baru**
    Sebuah branch bernama `eksperimen-styling` dibuat dan langsung dialihkan.
    ```bash
    git checkout -b eksperimen-styling
    ```

2.  **Melakukan Perubahan**
    Di dalam branch ini, dilakukan perubahan skema warna utama (variabel `--primary-color` di CSS) dari oranye menjadi biru.

3.  **Commit di Branch Eksperimen**
    Perubahan tersebut disimpan dalam sebuah commit khusus di branch `eksperimen-styling`.
    * **Pesan Commit:** `style: Eksperimen dengan skema warna biru`

### Fase 3: Menggabungkan Branch (Merge)

Setelah eksperimen dianggap berhasil, perubahan dari branch `eksperimen-styling` digabungkan kembali ke branch utama.

1.  **Kembali ke Branch Utama**
    ```bash
    git checkout main
    ```
2.  **Menggabungkan Perubahan**
    ```bash
    git merge eksperimen-styling
    ```
    Hasilnya, branch `main` kini memiliki skema warna biru yang baru.

### Fase 4: Publikasi ke GitHub

Tahap terakhir adalah mempublikasikan seluruh riwayat kerja ke repository remote di GitHub.

1.  **Menghubungkan ke Remote Repository**
    ```bash
    git remote add origin [https://github.com/](https://github.com/)[Nama-Username-Anda]/[nama-repositori-anda].git
    ```
2.  **Push ke GitHub**
    Seluruh commit dari branch `main` diunggah ke GitHub.
    ```bash
    git push -u origin main
    ```
### 
### Visualisasi Riwayat Commit (`git log`)

Berikut adalah bukti visual dari seluruh alur kerja yang dijalankan, diambil dari output perintah `git log --graph --oneline`:
---


Dibuat oleh **[Nama Lengkap Anda]** sebagai bagian dari tugas akhir mata kuliah Dasar Pemrograman Web.
