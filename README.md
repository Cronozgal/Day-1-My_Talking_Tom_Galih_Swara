# Catatan Workshop: Building with AI & Managing Change with GitHub

Disusun oleh: **Galih Swara**

---

## Tentang Repositori Ini
Repositori ini memuat arsip komprehensif, ringkasan materi, dan kode sumber dari proyek praktik yang dikerjakan selama workshop. Fokus utama dari acara ini adalah pemanfaatan kecerdasan buatan (AI) dalam menyusun perangkat lunak, serta pengelolaan versi proyek secara terstruktur lewat Git dan GitHub.

---

## Tujuan Pembuatan Repositori
Repositori ini dibangun untuk mencapai beberapa sasaran berikut:
1. **Arsip Pembelajaran:** Sebagai sentra penyimpanan dokumen dan catatan ilmu yang didapatkan sepanjang kegiatan.
2. **Implementasi *Version Control*:** Mengaplikasikan langsung alur kerja pengelolaan revisi kode (Git) sekaligus mengintegrasikannya dengan layanan GitHub.
3. **Koleksi Portofolio:** Menyimpan draf proyek latihan akhir ("*Student Task Planner*") agar dapat dijadikan acuan eksplorasi dan evaluasi di masa mendatang.

---

## Detail Kegiatan
- **Tema Acara:** Building with AI, Managing Change with GitHub
- **Narasumber:** Nugi Farhan (Senior Product Designer / UX Advisor)
- **Fokus Materi:**
  - Pengenalan teknik *Prompt Engineering* untuk mengoptimalkan penggunaan AI.
  - Tata kelola kolaborasi dan manajemen kode melalui Git & GitHub.
- **Proyek Latihan:** Mengembangkan purwarupa aplikasi *Student Task Planner* berbekal instruksi AI, dengan sistem penyimpanan berbasis Git/GitHub.

---

## Rangkuman Materi Workshop

### 1. Membangun Bersama AI (*Prompt Engineering*)
- **Definisi *Prompt* AI:** Perintah, instruksi, atau data masukan yang dikirim ke model AI guna memicu hasil keluaran yang spesifik.
- **Urgensi Konteks:** AI membutuhkan latar belakang yang utuh (tujuan, spesifikasi, dan batasan) agar mampu menyajikan solusi yang relevan dan akurat.
- **Anatomi *Prompt* yang Ideal:**
  - **Role:** Menetapkan identitas/profesi bagi AI.
  - **Task:** Menjabarkan instruksi utama yang perlu dieksekusi.
  - **Context:** Menyajikan informasi pendukung terkait tugas.
  - **Format/Output:** Mendefinisikan bentuk hasil akhir yang diharapkan.
- **Manfaat *Prompt Engineering*:** Memaksimalkan kualitas jawaban AI, menekan risiko bias atau misinformasi, meningkatkan akurasi respons (*predictability*), serta menyempurnakan interaksi pengguna.

### 2. Mengelola Perubahan dengan Git & GitHub
- **Git vs GitHub:**
  - **Git:** Sistem pengontrol versi terdistribusi (DVCS) di lingkungan lokal untuk merekam jejak revisi kode.
  - **GitHub:** Layanan *cloud* untuk menghosting repositori Git agar mudah diakses secara tim.
- **Alur Kerja Git (*Workflow*):**
  1. **Working Directory:** Ruang kerja tempat file diedit atau ditambahkan.
  2. **Staging Area (Index):** Zona transit untuk mendaftarkan file sebelum dikunci ke dalam rekaman riwayat.
  3. **Git Directory (Repository):** Basis data tempat Git menyimpan histori (*commit*) dan metadata proyek.
- **Kumpulan Perintah Esensial:**
  - *Lokal:* `git init` (memulai), `git add .` (memasukkan ke *staging*), `git commit -m "pesan"` (menyimpan riwayat).
  - *Integrasi Remote:* `git remote add <nama> <url>` (menyambungkan *remote*), `git push origin main` (mengunggah), `git pull origin main` (mengunduh).
- **Persiapan Awal (*Setup*):**
  - Mengatur identitas *developer* (`user.name` & `user.email`).
  - Menghubungkan *Command Line Interface* (CLI) dengan VS Code.
  - Membuat kunci SSH (`ssh-keygen -t ed25519`) dan menautkannya ke GitHub untuk keamanan autentikasi.

---

## Panduan Praktik: Membuat *Student Task Planner*
Langkah-langkah iterasi proyek selama sesi latihan:
1. Memanfaatkan layanan asisten AI (seperti Claude atau ChatGPT).
2. Menyusun *prompt* secara detail (mencakup peran, sasaran, spesifikasi, batasan, dan keluaran).
3. Memulai repositori lokal lewat perintah `git init`.
4. Menyimpan revisi (*commit*) perdana dan mengunggahnya (*push*) ke repositori daring.
5. Melakukan pembaruan kode dan penambahan fitur secara bertahap, lalu rutin mengeksekusi tahapan *commit* dan *push*.

---

## Wawasan Baru & Poin Penting (*Key Takeaways*)
- **Detail Konteks Menentukan Kualitas:** Menyematkan aturan (*constraints*) dan kriteria pokok (*requirements*) akan mencegah AI memberikan kode sampah (*bloatware*) atau *library* yang tidak dibutuhkan proyek.
- **Konsep Tiga Zona Git:** Perubahan kode tidak seketika masuk ke riwayat repositori. Semua file harus melewati transisi dari *Working Directory* $\rightarrow$ *Staging Area* $\rightarrow$ *.git Directory*.
- **Keamanan Tanpa Repot Berkat SSH:** Menerapkan SSH Key (khususnya varian Ed25519) adalah solusi termudah dan paling aman untuk menghubungkan mesin lokal ke GitHub, karena menghapus kewajiban mengetik *password* berulang kali.
- **Disiplin *Version Control*:** Biasakan untuk melakukan *commit* pada setiap penambahan fitur kecil atau perbaikan kode. Cantumkan pesan *commit* yang deskriptif supaya jejak tumbuh kembang aplikasi tersusun dengan sistematis dan mudah dilacak.
