# Halo, Selamat Datang! 🙋‍♂️

Repository ini berisi panduan workshop GitHub untuk peserta.

---

## 📌 Challenge Kelompok: Mission: Build & Publish

### 📝 Deskripsi

Challenge ini bertujuan menguji pemahaman peserta dalam menggunakan Git & GitHub untuk kolaborasi tim. Peserta akan membuat repository bersama, melakukan branching, commit oleh semua anggota, serta mempublikasikan hasil akhir menggunakan GitHub Pages.

**Setiap anggota kelompok diharapkan:**
- Mampu melakukan setup repo dan konfigurasi dasar.
- Melakukan kolaborasi nyata dengan branching & commit.
- Menyusun file proyek sederhana yang dapat ditampilkan sebagai website.
- Memahami proses merge dan publikasi melalui GitHub Pages.
- Menunjukkan kerja sama tim.

---

### 📂 Instruksi Challenge

1. Setup Repository & Struktur Folder (5 poin)
    - Buat repository baru bernama `workshop-github-2025`.
    - Tambahkan file `README.md` berisi:
      - Nama lengkap semua anggota.
      - Deskripsi singkat proyek (1–2 kalimat).
    - Buat struktur folder seperti berikut:
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

2. Kolaborasi Dasar (10 poin)
    - Setiap anggota wajib melakukan minimal 1 commit.
    - Buat branch baru bernama `fitur-kelompok`.

3. Isi Proyek (10 poin)
    - Catatan: Bagian ini hanya contoh, bukan patokan wajib. Silakan sesuaikan konten; yang penting mengikuti struktur folder yang sudah ditentukan.
    - Buat file utama index.html (contoh):
        ```html
        <!doctype html>
        <html lang="id">
            <head>
                <meta charset="utf-8" />
                <meta name="viewport" content="width=device-width, initial-scale=1" />
                <title>Workshop GitHub 2025</title>
                <link rel="stylesheet" href="style.css" />
            </head>
            <body>
                <h1 id="title">Hello GitHub Workshop</h1>
                <script defer src="script.js"></script>
            </body>
        </html>
        ```
    - Tambahkan style.css untuk styling sederhana (contoh):
        ```css
        body { font-family: system-ui, -apple-system, Segoe UI, Roboto, sans-serif; margin: 2rem; }
        h1 { color: #2563eb; text-align: center; }
        ```
    - Tambahkan script.js untuk interaktivitas sederhana (contoh):
        ```js
        document.addEventListener('DOMContentLoaded', () => {
            const title = document.getElementById('title');
            title.addEventListener('click', () => {
                title.textContent = 'Selamat datang di GitHub Pages!';
            });
            console.log('Script aktif');
        });
        ```
    - Perbarui docs/laporan.md: ringkasan proyek, daftar anggota, pembagian tugas, cara menjalankan, dan URL GitHub Pages.
    - Commit semua perubahan lewat branch fitur-kelompok (minimal 1 commit per anggota). Contoh:
        ```bash
        git add .
        git commit -m "feat: tambah index.html, style.css, script.js, dan laporan"
        git push origin fitur-kelompok
        ```

4. Merging (5 poin)
    - Lakukan merge branch `fitur-kelompok` ke branch utama `main`.

5. Publikasi GitHub Pages (wajib)
    - Aktifkan GitHub Pages pada repository.
    - Settings → Pages → pilih branch `main` → folder `/root`.
    - Pastikan file `index.html` dapat diakses publik.
    - Serahkan URL GitHub Pages kepada panitia.

---

### 📜 Template Laporan

Template laporan dapat ditemukan pada folder [docs](docs/laporan.md).
