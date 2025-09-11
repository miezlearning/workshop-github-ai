# 📌 Challenge Kelompok: Mission: Build & Contribute

### 📝 Deskripsi

Challenge ini bertujuan menguji pemahaman peserta dalam menggunakan Git & GitHub untuk kolaborasi tim dengan alur **open source contribution**.
Setiap anggota akan belajar membuat **fork**, bekerja di branch sendiri, lalu mengajukan perubahan lewat **Pull Request (PR)** ke repository utama.

**Setiap anggota kelompok diharapkan:**

* Memahami alur *fork → clone → branch → commit → push → pull request → merge → pull*.
* Melakukan kontribusi nyata melalui branching & commit.
* Menyusun file proyek sederhana sesuai struktur yang ditentukan.
* Memahami proses review dan sinkronisasi.
* Menunjukkan kerja sama tim.

---

### 📂 Instruksi Challenge

1. **Setup Repository Utama (5 poin)**

   * **Ketua** sudah menyiapkan repo publik bernama `workshop-team-2025`.
   * Repo utama berisi struktur folder awal dan file `README.md` kosong.
   * Ketua membagikan URL repo utama ke semua anggota kelompok.

2. **Fork & Clone (10 poin)**

   * **Setiap anggota** melakukan **Fork** repo utama ke akun GitHub masing-masing.
   * Clone hasil fork ke lokal:

     ```bash
     git clone <URL_fork_anda>
     cd workshop-team-2025
     ```
   * Tambahkan remote `upstream` yang menunjuk ke repo utama:

     ```bash
     git remote add upstream <URL_repo_utama>
     git remote -v
     ```

3. **Buat Branch & Kerjakan Proyek (10 poin)**

   * Buat branch baru dengan format `fitur/nama`.

     ```bash
     git switch -c fitur/nama
     ```
   * Tambahkan atau modifikasi file sesuai struktur proyek:

     ```
     workshop-github-2025/
     ├── README.md
     ├── index.html
     ├── style.css
     ├── script.js
     ├── docs/
     │   └── laporan.md
     └── assets/
     ```
   * Contoh commit:

     ```bash
     git add .
     git commit -m "feat: tambah profil Nama di script.js"
     git push origin fitur/nama
     ```

4. **Ajukan Pull Request (10 poin)**

   * Buka repo fork di GitHub → klik **“Compare & pull request”**.
   * Pastikan:
     * Base repo: `workshop-team-2025` (repo utama) → branch `main`.
     * Head repo: fork Anda → branch `fitur/nama`.
   * Beri judul PR jelas, contoh:
     `feat: tambah halaman profil Nama`.
   * Submit PR → tunggu review & merge.

5. **Merging (5 poin)**

   * **Ketua** mereview setiap PR anggota.
   * Jika sesuai, PR akan di-*merge* ke branch utama `main`.

6. **Sinkronisasi (5 poin)**

   * Setelah PR diterima, **semua anggota** melakukan update repo lokal agar sinkron dengan repo utama:

     ```bash
     git pull upstream main
     ```

---

### 📜 Bukti Hasil

* Setiap anggota wajib menunjukkan bahwa kontribusinya sudah di-*merge* dan namanya tercatat di tab **Contributors** repo utama.
* `docs/laporan.md` harus diperbarui berisi daftar anggota + link PR masing-masing.


### 📜 Template Laporan

Template laporan tersedia pada folder [docs](../docs/laporan.md).
