# Website Rute Angkot

## Bab 1 Pengenalan Website Rute Angkot<br />

### 1.1 APA ITU WEBSITE RUTE ANGKOT<br />

Website rute angkot adalah platform digital yang menyediakan informasi tentang rute angkutan kota (angkot) dalam bentuk tabel. Website ini memungkinkan pengguna untuk mencari dan menampilkan rute angkot yang tersedia di suatu kota, serta memberikan informasi detail mengenai jalur yang dilalui dan titik pemberhentian.<br />

### 1.2 Tujuan dan Manfaat Website Rute Angkot<br />

Dengan adanya website rute angkot, masyarakat dapat dengan mudah menemukan rute angkot yang mereka butuhkan, mengurangi ketergantungan pada informasi manual, dan meningkatkan efisiensi dalam penggunaan angkutan umum. Platform ini juga dapat membantu pemerintah dan operator angkutan kota dalam mengelola dan mengoptimalkan rute angkot.

## Bab 2 Metodologi Pembuatan Website<br />

### 2.1 BAHASA PEMOGRAMAN<br />

Dalam pengembangan suatu website, pemahaman terhadap bahasa pemograman menjadi kunci utama untuk dikuasai. Seperti saat membuat sebuah Website Rute Angkot, terdapat dua bahasa pemograman yang digunakan, yaitu Front-end dan Back-end. Front-end disini bertugas untuk memberikan tampilan antar pengguna, sedangkan Back-end bertugas untuk mengatur bagian server dari sebuah website.<br />
Front-end disini akan menggunakan JavaScript dan juga Framework CSS Skeleton. Dan untuk Back-end akan menggunakan bahasa GO.

#### 2.1.1 FRONTEND<br />

Frontend merupakan bagian pengembangan aplikasi web yang mencakup teknologi yang berinteraksi langsung dengan pengguna. Teknologi ini biasanya dikembangkan menggunakan HTML, CSS, JavaScript, dan alat desain grafis seperti Photoshop dan Fireworks. Tujuan pengembangan front-end adalah untuk menciptakan antarmuka pengguna grafis (GUI) yang memberikan pengalaman pengguna yang baik bagi pengguna akhir.(Jesús & Caballero, n.d.)<br />

#### 2.1.2 BACKEND<br />

“Backend” mewakili elemen sisi server dalam kerangka web yang berfungsi sebagai mediator antara klien dan repositori data, seperti database, cache Redis, atau penyimpanan blob. Ini bertanggung jawab untuk mengelola logika operasional, manipulasi data, dan komunikasi dengan database atau aset tambahan yang penting untuk mendukung aplikasi berbasis web.(Morozov, 2020)<br />

#### 2.1.3 HTML<br />

HTML Hypertext Markup Language berfungsi sebagai bahasa markup yang digunakan untuk pembuatan dokumen di internet. Dokumen di web biasanya dapat dijangkau melalui protokol HTTP, memfasilitasi transmisi data dari server situs web tertentu ke pengguna untuk visualisasi melalui browser web. Berfungsi sebagai bahasa markup, HTML menggunakan tag untuk menginstruksikan browser web tentang pemrosesan teks, sehingga menunjukkan apakah teks merupakan paragraf, daftar, atau hyperlink.(Rahmatika et al., 2021)<br />
Selain itu, HTML sering berfungsi sebagai tahap awal dalam pengembangan situs web dan dianggap penting bagi pemula yang memulai pembuatan situs web untuk memahami tag dasar dalam HTML.<br />

#### 2.1.4 CSS<br />

CSS adalah alat umum bagi pengembang web untuk mengontrol tampilan halaman web. Ini membantu menentukan ukuran teks, font, dan warna di seluruh situs. Ini memisahkan gaya dokumen dari struktur. CSS memungkinkan pengaturan font, warna, dan ukuran teks dalam HTML. Pengguna dapat menerapkan style sheet untuk menyesuaikan tampilan halaman web.(Burkhard, 2022)<br />

### 2.2 APLIKASI YANG DIGUNAKAN<br />

### 2.3 PENYIMPANAN YANG DIGUNAKAN<br />

## Bab 3 Perancangan dan Pengembangan Sistem<br />

## Bab 4 Tutorial Pembuatan Website<br />

### 4.1 Cara Connect Database MongoDB untuk Visual Studio Code <br />

Berikut adalah beberapa tutorial yang bisa membantu kalian dalam cara meng-connect database MongoDB ke visual studio code, dan cara menggunakan Mongostring.

#### 4.1.1 Cara membuat account MongoDB <br />

Buka browser default kalian dan cari di kolom pencarian MongoDB
setelah itu kalian akan di arahkan ke halaman web seperti gambar dibawah ini.
![Gambar1](<Images/Screenshot (385).png>)
Kalian bisa langsung click button “Try Atlas Free” dan kalian akan di arahkan ke halaman web seperti gambar dibawah ini.
![Gambar2](<Images/Screenshot (394).png>)
Setelah melakukan login/sign up maka kita bisa ke langkah berikutnya.

#### 4.1.2 Membuat cluster pada MongoDB dan menginstall Mongodb Compass <br />

Setelah membuat account, kalian akan di arahkan ke halaman web seperti gambar dibawah ini.
![Gambar3](<Images/Screenshot (388).png>)

Isilah form berikut sesuai kebutuhan kalian seperti kebutuhan organisasi, project, dsb. Setelah mengisi form tersebut silahkan click button “Finish” dan sebelum membuat cluster nya kita harus men-download yang namanya MongoDB Compass terlebih dahulu agar cluster nya dapat digunakan.
Tambahkan halaman web baru dan masukan MongoDB Compass ke dalam kolom pencarian browser kalian, setelah itu kalian akan dihadapkan dengan halaman web seperti gambar dibawah ini.
![Gambar4](<Images/Screenshot (386).png>)

Lalu kalian bisa click button “Download Now” dan kalian akan di arahkan ke halaman web Donwloadnya.
![Gambar5](<Images/Screenshot (387).png>)

Seperti yang kalian lihat pada gambar di atas, silahkan men-download MongoDB Compass (GUI) nya dan tunggu beberapa menit untuk menyelesaikan downlaod-an tersebut. Dan untuk pengguna macOS kalian bisa men-downlaodnya juga dengan cara mengubah platformnya dan sesuaikan dengan versi macOS kalian. Setelah download-an kalian selesai, kalian bisa kembali ke halaman web MongoDB Atlas nya untuk membuat cluster.
![Gambar6](<Images/Screenshot (385).png>)

Lengkapi Username dan Password kalian, setelah kalian lengkapi silahkan click button “Create Database User”
Setelah sudah meng-create database user kalian akan di hadapkan dengan seperti gambar dibawah ini.
![Gambar7](<Images/Screenshot (397).png>)

Kalian bisa meng-click button “Choose a connection method” untuk mendapatkan Mongostring nya.
![Gambar8](<Images/Screenshot (398).png>)

Seperti gambar di atas karena kalian sudah men-download MongoDB Compass kalian bisa memilih “Access your data trhough tools Compass”.
![Gambar9](<Images/Screenshot (399).png>)

Setelah kalian memilih tools menggunakan compass kalian akan di arahkan seperti gambar di atas, kalian tinggal memilih “I have MongoDB compass installed” karena kalian sudah men-down;oad nya tadi, dan di bawahnya akan tertera connection string nya. Ini yang akan dipakai ketika kita memakai software MongoDB compass nya,tidak lupa untuk meng-copy connection string nya dan simpan baik-baik karena akan selalu dipakai ketika anda sedang menggunakan MongoDB Compass, sekarang menuju langkah terakhir.

#### 4.1.3 Cara menambahkan New Connection di dalam MongoDB Compass. <br />

Pertama buka software MongoDB Compass kalian yang sudah terinstall.
![Gambar10](<Images/Screenshot (400).png>)
Setelah itu click button “New Connection” lalu tambahkan connection string yang telah kamu copy dari MongoDB Atlas sebelumnya, lalu silahkan click button “Connect”.

![Gambar11](<Images/Screenshot (401).png>)
Dan Selamat kalian sudah bisa menggunakan MongoDB Compass kalian, sedangkan untuk meng-connect di dalam VCS (Visual Studia Code) kalian harus menambahkan mongostring nya kedalam codingan kalian misal seperti gambar dibawah ini.
![Gambar12](<Images/Screenshot (402).png>)
Jika sudah menambahkan connection string nya kalian bisa langsung meng-run codingan tersebut, karena saya menggunakan bahasa golang jadi untuk meng-run codingannya harus memakai perintah “Go-run nama file yang akan di run” seperti ini di terminal kalian. Contoh nya seperti gambar dibawah ini.
![Gambar12](<Images/Screenshot (403).png>)
Jika codingan kalian saat di run menghasilkan hasil yang seperti pada gambar di atas, maka selamat codingan anda sudah connect dengan MongoDB.
NB:
Jika kalian ingin menambahkan database mengaturnya itu lewat MongoDB Compass sedangkan web service nya ada di MongoDB Atlas.

