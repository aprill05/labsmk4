Berikut adalah panduan dasar untuk membuat aplikasi web sederhana menggunakan Node.js:

1. Persiapkan Proyek:
Buat direktori untuk proyek Anda dan masuk ke dalamnya melalui terminal atau command prompt.

bash
Copy code
mkdir proyek-nodejs
cd proyek-nodejs

2. Inisialisasi Proyek Node.js:
Jalankan perintah berikut untuk membuat berkas package.json yang akan menyimpan informasi konfigurasi proyek dan daftar dependensi:

bash
Copy code
npm init -y

3. Instalasi Express:
Express.js adalah kerangka kerja (framework) Node.js yang populer untuk membangun aplikasi web. Instal Express dengan menggunakan perintah berikut:

bash
Copy code
npm install express
Buat Berkas App.js:
Buat berkas app.js sebagai titik masuk (entry point) aplikasi Anda. Gunakan teks editor untuk membuat berkas ini.


4. javascript
Copy code
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Selamat datang di aplikasi web Node.js!');
});

app.listen(port, () => {
  console.log(`Aplikasi berjalan di http://localhost:${port}`);
});
Dalam contoh ini, aplikasi memiliki satu route (beranda) yang mengirimkan respons dengan pesan sederhana.


5. Jalankan Aplikasi:
Kembali ke terminal dan jalankan aplikasi dengan perintah:

bash
Copy code
node app.js
Buka browser dan kunjungi http://localhost:3000 untuk melihat pesan selamat datang.

6. Menggunakan Template Engine (Opsional):
Jika Anda ingin membuat halaman web dinamis, Anda bisa menggunakan template engine seperti EJS atau Pug. Install salah satu template engine tersebut:

bash
Copy code
npm install ejs
Kemudian, ubah app.js untuk menggunakan template engine:

javascript
Copy code
const express = require('express');
const app = express();
const port = 3000;

app.set('view engine', 'ejs');

app.get('/', (req, res) => {
  res.render('index', { message: 'Selamat datang di aplikasi web Node.js!' });
});

app.listen(port, () => {
  console.log(`Aplikasi berjalan di http://localhost:${port}`);
});
Buat berkas views/index.ejs dengan konten:

html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Web Node.js</title>
</head>
<body>
  <h1><%= message %></h1>
</body>
</html>
Dengan menggunakan EJS, Anda dapat memasukkan data dinamis ke dalam halaman web.

