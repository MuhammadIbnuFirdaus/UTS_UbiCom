
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Automatic Space Parking using CCTV(Dronify) Project Ubiquitous Computing</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/default.min.css">
    <link rel="stylesheet" href="/styles/style.css"> 

    <script defer src="https://cdn.jsdelivr.net/npm/alpinejs@3.x.x/dist/cdn.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"></script>

    <script type="module">
      import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
    </script>

    <script src="/scripts/default.js"></script>
    <script>
      hljs.highlightAll();
    </script>
  </head>
  <body>
    <div class="top-menu">
      <a href="/">Home</a>
      <a href="/courses">Courses</a>
      <a href="/rnd">RnD</a>
      <a href="/blog">Blog</a>
    </div> 
  
    <div class="container mt-2">
      <a href="/courses/ubicom">
        &laquo; Ubiquitous Computing
      </a>
      <h1>
        <a href="/courses/ubicom/contoh-format-project">
          Contoh Format Project Ubiquitous Computing
        </a>
      </h1>
      <a href="/">Muhammad Insan Al-Amin</a> - Oct 9, 2023
    </div>

    <div class="container mt-4">
      <div x-init="" x-html="mdToHTML($el.innerHTML)" class="row mt-2">
## Intro 
- Artikel ini membahas pembangunan teknologi Ubiquitous Computer yang Menyusun tema Automatic Detection Space Parking using CCTV Camera Technology pada sebuah universitas.

 

## Latar Belakang 
Pada tahap ini kita menunjukan alasan utama mengapa membuat produk UbiCom ini. Contoh isi:
•	Menurut CCN Indonesia jumlah kendaraan bermotor pada januari 2023 mencapai 150 juta unit kendaraan bermotor, dan seiring berjalannya waktu jumlahnya akan semakin bertambah. Dan dari beberapa mahasiswa juga sering terlambat masuk kelas dikarenakan mencari lahan parkir, dan mengeluh akan kesulitannya mencari lahan parkir yang aman dan efisien yang dekat dari gedung perkuliahan.
•	Dengan adanya beberapa CCTV di berbagai titik parkiran pada sebuah gedung universitas bisa saja dijadikan sebuah solusi sebagai alat pendeteksi parkiran untuk mahasiswa, yang dimana nantinya mahasiswa hanya cukup membuka smartphone mereka dan login ke website atau lms kampus mereka dan mencari parkiran yang terdekat dengan gedung perkuliahan mereka.

 

## Branding 
Pada tahap ini kita mengeksplorasi branding dari produk UbiCom yang dibuat. Contoh:
•	Merk: Website atau LMS Universitas
•	Inspirasi merk: Menambahkan fitur menu cari parkir untuk mahasiswa mencari lahan parkir yang terdekat dengan gedung mereka. 
•	Tagline: -
•	Campaign: Menjadikan sebuah CCTV yang bukan hanya sekedar CCTV tetapi juga bisa mendeteksi keberadaan kendaraan pada lahan parkir.
•	Target user:
o	Usia 17+
o	Mahasiswa kampus yang membawa kendaraan
•	User experience theme:
o	Mudah dikonfigurasi dan digunakan
o	Berbasis mobile agar mudah di gunakan.



## User Story
Pada tahap ini kita mengeksplorasi kebutuhan prioritas dari para pengguna untuk kita wujudkan sebagai fitur pada sistem atau aplikasi yang akan dibuat. User story memudahkan kita membuat prioritas fitur-fitur untuk dikerjakan untuk jangka waktu tertentu.

|Sebagai|Saya ingin bisa|Sehingga|Prioritas
|---|---|---|---|
|Sebagai Pengguna|Bisa digunakan oleh semua device|Lebih Praktis|⭐⭐⭐⭐⭐|
|Sebagai Pengguna|Menggunakan satu platform baik itu website maupun aplikasi|Tidak banyak membuka bnyak aplikasi|⭐⭐⭐⭐⭐|
|Sebagai Sistem|Merekognisi kondisi lahan parkir secara real time|Pengguna bisa menggunakan kapan saja|⭐⭐⭐⭐|

## Metode dan Algoritma 
Pada tahap ini kita menjelaskan metode dan algoritma yang digunakan pada setiap komponen teknologi UbiCom. Contoh:
- Sensor:
  - Video detection: Feed Video. Kamera CCTV dengan perangkat lunak pengenalan gambar dapat digunakan untuk menghitung jumlah kendaraan dengan mengenali gambar kendaraan.!

- Responder:
  - YOLO
  - Fuzzy Logic

## Struktur Data 
Pada tahap ini kita mengeksplorasi struktur data yang digunakan pada teknologi UbiCom. Contoh:
<img width="239" alt="Screenshot 2023-12-27 at 15 21 40" src="https://github.com/MuhammadIbnuFirdaus/UTS_UbiCom/assets/101255568/5b29b0e5-0271-4b8d-8192-ab212ce26080">


- Pada tahap ini kita mengeksplorasi dan menganalisis bentuk struktur data yang mampu memfasilitasi *user story* yang ada, maupun yang kemungkinan besar dibutuhkan di kemudian hari
- Kita akan merepresentasikan Entitas pada aplikasi dalam bentuk tabel Entitas dan Atribut

## Arsitektur Sistem 
<img width="289" alt="image" src="https://github.com/MuhammadIbnuFirdaus/UTS_UbiCom/assets/101255568/cad01c32-f765-4b23-bce7-75d5e17bd620">


Pada tahap ini kita merancang arsitektur berikut teknologi yang terdapat pada setiap komponen pembentuk aplikasi.

## Deskripsi Teknologi 
Pada tahap ini kita menjelaskan setiap teknologi hardware dan software yang digunakan dalam pembangunan sistem. Contoh:
1.	Python: Sebagai mesin komputasi. Alasan menggunakan phyton memiliki secourse yang sangat luas, pengoprasian yang flexible dan mudah dipahami
2.	OpenCV: Sebagai Pengelolaan atau menyediakan algoritma untuk mendeteksi dan melacak objek baik itu gambar ataupun video
3.	Visual Studio Code / Google Collab: Sebagai teks editor
4.	Sensor: CCTV: Merk Hikvision. adalah produsen CCTV yang menawarkan solusi mendukung teknologi Space Parking Detection.


## User Experience (UX) Design 

Mock up sederhana
<img width="537" alt="Screenshot 2023-12-08 at 02 47 13" src="https://github.com/MuhammadIbnuFirdaus/UTS_UbiCom/assets/101255568/d944cdc4-2c81-4b73-a26f-5a2df99743c6">

      </div>
    </div> 

  </body>
</html>
