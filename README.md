# Laporan Pengerjaan Tugas Akhir: Website Portofolio dengan Git Workflow
## Deskripsi Proyek

Website ini adalah portofolio statis yang dibangun menggunakan **HTML5** dan **CSS3**. Halaman ini menampilkan profil, kompetensi (skills), proyek-proyek unggulan, dan formulir kontak. Proyek ini dibuat sebagai latihan untuk menerapkan konsep dasar pengembangan web dan sistem kontrol versi (Git).

Berikut adalah dokumentasi langkah demi langkah dari proses pengerjaan proyek ini, sesuai dengan riwayat commit yang tercatat di Git.

### Fase 1: Inisialisasi dan Commit Bertahap

Proyek dimulai dengan inisialisasi repository Git lokal dan dilanjutkan dengan pembangunan website section per section. Setiap bagian yang selesai langsung di-commit untuk menciptakan riwayat perubahan yang logis.

1.  **Navigasi ke Direktori Proyek**
    Langkah pertama adalah membuka terminal dan masuk ke folder kerja proyek.
    ```bash
    cd d:/laragon/www/pemweb/portofolio-saya
    ```
    <img width="746" height="178" alt="Screenshot 2025-11-01 223952" src="https://github.com/user-attachments/assets/6fb2a444-950e-4f92-9a46-248e456647e2" />

2.  **Inisialisasi Proyek**
    Repository Git lokal dibuat di dalam folder proyek.
    ```bash
    git init
    ```
    <img width="774" height="71" alt="Screenshot 2025-11-01 235053" src="https://github.com/user-attachments/assets/cf402631-8ca8-4a25-b786-a6e4d8b2c1cb" />


3.  **Commit #1: Struktur Dasar**
    Membuat kerangka dasar HTML dan file CSS, termasuk pengaturan variabel warna, font global, dan reset CSS dasar.
    * **Pesan Commit:** `Inisialisasi proyek dengan struktur HTML & CSS dasar`
    <img width="751" height="178" alt="image" src="https://github.com/user-attachments/assets/6ed7b438-0951-4f5e-b24b-c69f85f9f5fc" />


4.  **Commit #2: Header & Navigasi**
    Menambahkan bagian `<header>` yang berisi logo dan menu navigasi utama.
    * **Pesan Commit:** `Tambah section header dan navigasi`
    <img width="706" height="130" alt="Screenshot 2025-11-01 231355" src="https://github.com/user-attachments/assets/ae43e50e-e826-4c27-a720-b3a5190bb0a1" />

5.  **Commit #3: Section 'About'**
    Membuat section "Tentang Saya" yang berisi perkenalan diri, foto, dan tombol ajakan (call-to-action).
    * **Pesan Commit:** `buat section 'Tentang Saya' (About)`
    <img width="724" height="140" alt="Screenshot 2025-11-01 231359" src="https://github.com/user-attachments/assets/e49e71ed-15cf-413a-9339-2de2e835fd8a" />

6.  **Commit #4: Section 'Skills'**
    Menambahkan section "Kompetensi" yang menampilkan daftar bahasa pemrograman dan tools yang dikuasai dalam format kartu.
    * **Pesan Commit:** `buat section 'Kompetensi' (Skills)`
    <img width="697" height="130" alt="Screenshot 2025-11-01 231404" src="https://github.com/user-attachments/assets/d59f0b55-a1b5-484e-87e2-75b9cfa27f2c" />

7.  **Commit #5: Section 'Projects'**
    Membuat section "Proyek Unggulan" untuk menampilkan portofolio proyek yang pernah dikerjakan.
    * **Pesan Commit:** `buat section 'Proyek Unggulan' (Projects)`
    <img width="726" height="128" alt="Screenshot 2025-11-01 231409" src="https://github.com/user-attachments/assets/33948485-475d-40c7-8250-d5386a28cdae" />

8.  **Commit #6: Section 'Contact' & Footer**
    Menyelesaikan halaman dengan menambahkan formulir kontak dan `<footer>`.
    * **Pesan Commit:** `Tambah section 'Kontak' dan footer halaman`
    <img width="749" height="139" alt="Screenshot 2025-11-01 231416" src="https://github.com/user-attachments/assets/ec498478-1fe9-4fde-b20f-5b19fb39fb22" />

### Fase 2: Eksperimen Styling dengan Branch

Untuk mencoba ide desain baru tanpa merusak kode utama yang sudah stabil, sebuah branch baru dibuat.

1.  **Membuat Branch Baru**
    Sebuah branch bernama `eksperimen-styling` dibuat dan langsung dialihkan.
    ```bash
    git checkout -b eksperimen-styling
    ```
    <img width="734" height="58" alt="image" src="https://github.com/user-attachments/assets/22a152b5-061b-4afb-bf5c-6338f55bfe8a" />

2.  **Melakukan Perubahan**
    Di dalam branch ini, dilakukan perubahan skema warna utama (variabel `--primary-color` di CSS) dari oranye menjadi biru.

3.  **Commit di Branch Eksperimen**
    Perubahan tersebut disimpan dalam sebuah commit khusus di branch `eksperimen-styling`.
    * **Pesan Commit:** `style: Eksperimen dengan skema warna biru`
    <img width="730" height="175" alt="image" src="https://github.com/user-attachments/assets/b67478a3-73d3-4612-b9e1-3407bc368414" />


### Fase 3: Menggabungkan Branch (Merge)

Setelah eksperimen dianggap berhasil, perubahan dari branch `eksperimen-styling` digabungkan kembali ke branch utama.

1.  **Kembali ke Branch Utama**
    ```bash
    git checkout main
    ```
    <img width="761" height="74" alt="Screenshot 2025-11-01 231809" src="https://github.com/user-attachments/assets/79e1d50f-94c3-4dca-9cf8-b93685688376" />

2.  **Menggabungkan Perubahan**
    ```bash
    git merge eksperimen-styling
    ```
    <img width="719" height="106" alt="Screenshot 2025-11-01 231815" src="https://github.com/user-attachments/assets/db5c0333-c995-48d6-9b7a-72d8135db674" />

    Hasilnya, branch `master` kini memiliki skema warna biru yang baru.

### Fase 4: Publikasi ke GitHub

Tahap terakhir adalah mempublikasikan seluruh riwayat kerja ke repository remote di GitHub.

1.  **Menghubungkan ke Remote Repository**
    ```bash
    git remote add origin [https://github.com/](https://github.com/)[Nama-Username-Anda]/[nama-repositori-anda].git
    ```
    <img width="722" height="56" alt="image" src="https://github.com/user-attachments/assets/b3b7727a-a3ff-4c4a-bb52-fcc6ecc4765b" />

2.  **Push ke GitHub**
    Seluruh commit dari branch `main` diunggah ke GitHub.
    ```bash
    git push -u origin main
    ```
    <img width="717" height="262" alt="image" src="https://github.com/user-attachments/assets/eb62023e-1d59-4b4c-ba60-0ffd26f5c5ab" />

##  Langkah Instalasi & Penggunaan

Proyek ini bersifat statis dan tidak memerlukan proses instalasi yang rumit. Untuk menjalankannya di komputer lokal Anda:

1.  **Clone repository ini:**
    ```bash
    git clone https://github.com/Yoollaaa/tugas-akhir-portofolio.git
    ```

2.  **Masuk ke direktori proyek:**
    ```bash
    cd tugas-akhir-portofolio
    ```

3.  **Buka file `index.html`** di browser favorit Anda.

---
### 
### Visualisasi Riwayat Commit (`git log`)

Berikut adalah bukti visual dari seluruh alur kerja yang dijalankan, diambil dari output perintah `git log --graph --oneline`:
    <img width="923" height="168" alt="Screenshot 2025-11-01 233159" src="https://github.com/user-attachments/assets/e5218d29-2718-4bb2-b0da-91d4b08bab4b" />

---



