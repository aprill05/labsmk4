Membuat situs web statis di GitHub bisa dilakukan dengan menggunakan GitHub Pages. GitHub Pages adalah layanan hosting web yang disediakan oleh GitHub secara gratis.
Berikut langkah-langkah umum untuk membuat situs web statis di GitHub:

1. Buat Repository di GitHub:

* Buka halaman GitHub dan login ke akun Anda.
* Klik tombol "+", kemudian pilih "New repository".
* Beri nama repository Anda, misalnya "username.github.io" (ganti "username" dengan nama pengguna GitHub Anda).
* Pilih opsi "Public" agar situs web dapat diakses secara publik.
* Klik "Create repository".

 2. Tambahkan File HTML:

* Buat file HTML untuk situs web Anda.
* Anda dapat membuatnya menggunakan editor teks biasa seperti Notepad, Visual Studio Code, atau editor teks lainnya.
* Simpan file dengan nama index.html di dalam repository Anda.

3. Commit dan Push ke Repository:

* Buka terminal atau command prompt.
* Pindah ke direktori tempat Anda menyimpan file HTML.
* Inisialisasi repository Git dengan perintah git init.
* Tambahkan file ke repository dengan perintah git add ..
* Lakukan commit dengan perintah git commit -m "Initial commit".
* Hubungkan repository lokal dengan repository GitHub Anda dengan perintah git remote add origin https://github.com/username/username.github.
  io.git (ganti "username" dengan nama pengguna Anda).
* Push ke GitHub dengan perintah git push -u origin master.

4. Aktifkan GitHub Pages:

* Buka halaman repository di GitHub.
* Pilih tab "Settings".
* Gulir ke bawah ke bagian "GitHub Pages".
* Di bagian "Source", pilih "main branch" atau "master branch", tergantung pada versi Git yang Anda gunakan.
* Klik "Save".
