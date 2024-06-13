# Pengembangan Website Rute Angkot

## Chapter 1 Pengenalan Golang dan Javascript<br />

### 1.1 Defini Golang<br />

Go, juga dikenal sebagai Golang, adalah bahasa pemrograman yang dikembangkan oleh Google untuk membantu Anda menulis kode secara efisien dan mudah, aman, terukur, dan mudah dipelihara. Go dirancang untuk menyederhanakan manajemen ketergantungan dan proses pengembangan perangkat lunak. Bahasa ini secara asli mendukung konkurensi dan konkurensi, menjadikannya pilihan populer untuk pengembangan perangkat lunak yang memerlukan kinerja dan skalabilitas tinggi.(Blumen & Meyerson, n.d.)<br />

### 1.2 Defini Javascript<br />

JavaScript, bahasa pemrograman skrip yang banyak digunakan, memegang posisi penting dalam lanskap aplikasi web kontemporer. Bahasa ini, yang dicirikan oleh sifatnya yang dinamis, sistem pengetikan longgar, dan properti asinkron, mengambil peran penting dalam mengaktifkan fungsionalitas interaktif dalam platform berbasis web. Selain itu, JavaScript digunakan secara luas untuk memfasilitasi manipulasi real-time dan interaksi dengan Document Object Model (DOM), komponen penting dalam struktur halaman web.(Ocariza et al., 2015)<br />

### 1.3 Kelebihan menggunakan Golang dan Javascript dalam Pengembangan Web

#### Kelebihan Golang (Go)

1. Golang memiliki performa yang sangat baik karena dikompilasi menjadi kode mesin, sehingga berjalan lebih cepat dibandingkan bahasa yang diinterpretasikan seperti JavaScript.<br />
2. Golang memiliki dukungan bawaan yang sangat kuat untuk concurrency melalui goroutines dan channels, yang memudahkan pengembangan aplikasi dengan kemampuan pemrosesan paralel yang efisien.<br />
3. Golang adalah bahasa yang statically written, yang berarti banyak kesalahan bisa ditangkap pada saat kompilasi, sehingga mengurangi bug pada runtime.<br />
4. Sintaks Golang dirancang untuk sederhana dan mudah dibaca, yang membuatnya lebih mudah untuk dipelajari dan dipahami.<br />
5. Waktu kompilasi Golang sangat cepat dibandingkan dengan banyak bahasa lain yang dikompilasi, yang mempercepat siklus pengembangan.<br />
6. Golang memiliki ekosistem yang kuat dengan banyak pustaka dan alat bantu, serta komunitas yang aktif.<br />

#### Kelebihan JavaScript

1. JavaScript adalah bahasa pemrograman yang withering umum digunakan untuk pengembangan front-end web. Semua browser cutting edge mendukung JavaScript, membuatnya esensial untuk pengembangan aplikasi web interaktif.<br />
2. JavaScript memiliki ekosistem yang sangat luas dengan banyak system dan library populer seperti Respond, Precise, dan Vue.js untuk pengembangan front-end, serta Node.js untuk back-end.<br />
3. JavaScript memiliki dukungan kuat untuk offbeat programming dengan fitur seperti Guarantees, async/await, dan event-driven programming, yang penting untuk pengembangan aplikasi web present day yang responsif.<br />
4. JavaScript memiliki komunitas pengembang yang sangat besar dan aktif, yang menyediakan banyak sumber daya, instructional exercise, dan alat bantu untuk pengembangan web.<br />
5. JavaScript memungkinkan pembuatan aplikasi web yang dapat memperbarui konten secara real-time tanpa perlu memuat ulang halaman, berkat teknologi seperti WebSockets dan system seperti Meteor.js.<br />

## Chapter 2 Persiapan Lingkungan Pengembang<br />

### 2.1 Cara Install Golang<br />

### 2.1 Setting up Visual Studio Code dan ekstensi yang diperlukan<br />

Visual Studio Code adalah editor kode sumber terbuka oleh Microsoft. Visual Studio Code mendukung berbagai bahasa pemrograman dan dikenal untuk fitur seperti debugging dan penyelesaian kode. Biasanya digunakan untuk pengembangan web dan berbasis cloud, berkat fleksibilitas dan perpustakaan ekstensinya. Editor menawarkan kontrol, manajemen build, pengujian unit, dan kemampuan pengujian statis. Dengan fitur-fitur ini, menjadikannya alat yang berharga bagi pengembang.(Murari & Sandru, 2013)

## Chapter 3 Membangun Backend dengan Golang <br />

“Backend” mewakili elemen sisi server dalam kerangka web yang berfungsi sebagai mediator antara klien dan repositori data, seperti database, cache Redis, atau penyimpanan blob. Ini bertanggung jawab untuk mengelola logika operasional, manipulasi data, dan komunikasi dengan database atau aset tambahan yang penting untuk mendukung aplikasi berbasis web.(Morozov, 2020)<br />

### 3.1 Struktur dasar Proyek Golang<br />

Golang (Go) adalah bahasa pemrograman yang dirancang untuk efisiensi, kecepatan, dan kesederhanaan. Dalam pengembangan aplikasi dengan Go, struktur proyek yang baik sangat penting untuk menjaga kode terorganisir, mudah dikelola, dan mudah dipahami oleh pengembang lain. Struktur proyek yang baik juga membantu dalam pemisahan tanggung jawab, memungkinkan pengujian yang lebih mudah, dan memfasilitasi kolaborasi antar tim.<br />

Struktur proyek Golang dapat bervariasi tergantung pada jenis aplikasi (misalnya, aplikasi web, layanan mikro, alat CLI), namun biasanya mengikuti pola umum. Berikut adalah struktur dasar dan penjelasan untuk masing-masing direktori dan file berdasarkan contoh yang Anda berikan: <br />
![Gambar](<Images/Screenshot (422).png>)<br />
Gambar di atas adalah contoh dari struktur golang bisa dilihat file apa saja yang wajib ada saat anda menggunakan bahasa golang. <br />

#### Penjelasan Direktori dan File

1. Cmd
   Direktori ini berisi aplikasi yang bisa dieksekusi. Subdirektori biasanya mengandung file "main.go" yang berfungsi sebagai entry point aplikasi.
   [Gambar](<Images/Screenshot (425).png>)
2. Internal
   Direktori ini berisi kode yang hanya boleh digunakan dalam proyek yang sama. Paket-paket di dalam "internal" tidak bisa diimpor oleh proyek lain.
   [Gambar](<Images/Screenshot (426).png>)<br />
3. Pkg
   Berisi paket-paket yang dapat diimpor oleh proyek lain atau oleh beberapa aplikasi dalam proyek yang sama. Ini adalah kode yang dapat digunakan ulang.
   [Gambar](<Images/Screenshot (427).png>)<br />
4. API
   Direktori ini digunakan untuk mendifinisikan API (misalnya, handler HTTP, spesifikasi API versi tertentu).
   [Gambar](<Images/Screenshot (429).png>)<br />
5. Web
   Berisi file statis (seperti CSS, JS) dan template HTML jika Anda memiliki aplikasi web.
   [Gambar](<Images/Screenshot (428).png>)<br />

<br />

### 3.2 Menghubungkan ke Database (MongoDB) <br />

MongoDB adalah database NoSQL yang menggunakan model dokumen, yang berarti data disimpan dalam format JSON-like yang fleksibel. MongoDB sangat cocok untuk aplikasi yang memerlukan skema dinamis dan dapat menangani berbagai jenis data. Keunggulan MongoDB termasuk skalabilitas yang mudah, performa tinggi, dan kemampuan untuk menangani data yang besar. Berikut adalah contoh dokumen MongoDB:
![Gambar](<Images/carbon(7).png>) <br />

![Gambar](<Images/carbon(8).png>) <br />

Langkah Pertama Buka browser default kalian dan cari di kolom pencarian MongoDB
setelah itu kalian akan di arahkan ke halaman web seperti gambar dibawah ini.
![Gambar1](<Images/Screenshot (385).png>)<br />
Kalian bisa langsung click button “Try Atlas Free” dan kalian akan di arahkan ke halaman web seperti gambar dibawah ini.
![Gambar2](<Images/Screenshot (394).png>)<br />
Setelah melakukan login/sign up maka kita bisa ke langkah berikutnya.

Setelah membuat account, kalian akan di arahkan ke halaman web seperti gambar dibawah ini.
![Gambar3](<Images/Screenshot (388).png>)<br />

Isilah form berikut sesuai kebutuhan kalian seperti kebutuhan organisasi, project, dsb. Setelah mengisi form tersebut silahkan click button “Finish” dan sebelum membuat cluster nya kita harus men-download yang namanya MongoDB Compass terlebih dahulu agar cluster nya dapat digunakan.
Tambahkan halaman web baru dan masukan MongoDB Compass ke dalam kolom pencarian browser kalian, setelah itu kalian akan dihadapkan dengan halaman web seperti gambar dibawah ini.
![Gambar4](<Images/Screenshot (386).png>)<br />

Lalu kalian bisa click button “Download Now” dan kalian akan di arahkan ke halaman web Donwloadnya.
![Gambar5](<Images/Screenshot (387).png>)<br />

Seperti yang kalian lihat pada gambar di atas, silahkan men-download MongoDB Compass (GUI) nya dan tunggu beberapa menit untuk menyelesaikan downlaod-an tersebut. Dan untuk pengguna macOS kalian bisa men-downlaodnya juga dengan cara mengubah platformnya dan sesuaikan dengan versi macOS kalian. Setelah download-an kalian selesai, kalian bisa kembali ke halaman web MongoDB Atlas nya untuk membuat cluster.
![Gambar6](<Images/Screenshot (385).png>)<br />

Lengkapi Username dan Password kalian, setelah kalian lengkapi silahkan click button “Create Database User”
Setelah sudah meng-create database user kalian akan di hadapkan dengan seperti gambar dibawah ini.
![Gambar7](<Images/Screenshot (397).png>)<br />

Kalian bisa meng-click button “Choose a connection method” untuk mendapatkan Mongostring nya.
![Gambar8](<Images/Screenshot (398).png>)<br />

Seperti gambar di atas karena kalian sudah men-download MongoDB Compass kalian bisa memilih “Access your data trhough tools Compass”.
![Gambar9](<Images/Screenshot (399).png>)<br />

Setelah kalian memilih tools menggunakan compass kalian akan di arahkan seperti gambar di atas, kalian tinggal memilih “I have MongoDB compass installed” karena kalian sudah men-down;oad nya tadi, dan di bawahnya akan tertera connection string nya. Ini yang akan dipakai ketika kita memakai software MongoDB compass nya,tidak lupa untuk meng-copy connection string nya dan simpan baik-baik karena akan selalu dipakai ketika anda sedang menggunakan MongoDB Compass, sekarang menuju langkah terakhir.

Pertama buka software MongoDB Compass kalian yang sudah terinstall.
![Gambar10](<Images/Screenshot (400).png>)<br />
Setelah itu click button “New Connection” lalu tambahkan connection string yang telah kamu copy dari MongoDB Atlas sebelumnya, lalu silahkan click button “Connect”.

![Gambar11](<Images/Screenshot (401).png>)<br />
Dan Selamat kalian sudah bisa menggunakan MongoDB Compass kalian, sedangkan untuk meng-connect di dalam VCS (Visual Studia Code) kalian harus menambahkan mongostring nya kedalam codingan kalian misal seperti gambar dibawah ini.
![Gambar12](<Images/Screenshot (402).png>)<br />
Jika sudah menambahkan connection string nya kalian bisa langsung meng-run codingan tersebut, karena saya menggunakan bahasa golang jadi untuk meng-run codingannya harus memakai perintah “Go-run nama file yang akan di run” seperti ini di terminal kalian. Contoh nya seperti gambar dibawah ini.
![Gambar12](<Images/Screenshot (403).png>)<br />
Jika codingan kalian saat di run menghasilkan hasil yang seperti pada gambar di atas, maka selamat codingan anda sudah connect dengan MongoDB.
NB:
Jika kalian ingin menambahkan database mengaturnya itu lewat MongoDB Compass sedangkan web service nya ada di MongoDB Atlas.

#### Berikut langkah-langkah untuk menghubungkan koneksi basis data mongodb <br />

Setelah menyiapkan MongoDB, langkah selanjutnya dalam pengembangan backend untuk website Rute Angkot adalah menghubungkan aplikasi backend dengan basis data tersebut. MongoDB adalah basis data NoSQL yang berbasis dokumen, yang menyimpan data dalam bentuk BSON (Binary JSON). Dalam langkah ini, kita akan membuat koneksi antara aplikasi backend dan MongoDB, serta menyiapkan skema dan model untuk data rute angkot.

Langkah pertama kalian bisa install Mongoose :
kalian bisa masuk ke file project kalian dan masuk ke visual studio code
![Gambar](<Images/Screenshot (412).png>)<br />
setelah itu kalian bisa buka terminal di dalam visual studio code dan saat berada di terminal kalian bisa mengetik command di terminal "npm install moongose" seperti gambar dibawah ini.
![Gambar](<Images/Screenshot (413).png>)<br />
![Gambar](<Images/Screenshot (414).png>)<br />
tunggu sampai proses downlaodnya selesai, setelah selesai kalian bisa langsung membuat file di dalam folder backend dan buat file "database.js".
![Gambar](<Images/Screenshot%20(418).png>)<br />
lalu isi codingan didalamnya dengan codingan seperti gambar dibawah ini atau kalian bisa atur sesuka hati kalian.
![Gambar](<Images/Screenshot%20(421).png>)<br />
setelah menambahkan file database kalian bisa buat file "app.js" seperti gambar dibawah ini.
![Gambar](<Images/Screenshot%20(419).png>)<br />
dan kalian bisa mengisi di dalam codingannya seperti ini.
![Gambar](<Images/Screenshot%20(420).png>)<br />

## Chapter 4 Membangun Frontend dengan Javascript <br />

### 4.1 Struktur dasar proyek Javascript

![Gambar](Images/directory%20front.png) <br />

Pada bagian Frontend, struktur direktori bisa disesuaikan sesuai keinginan. Namun, yang paling penting adalah dalam struktur ini terdapat tiga file HTML: satu untuk halaman utama, satu untuk halaman admin, dan satu untuk halaman login. Demikian juga dengan file CSS dan JavaScript, masing-masing terdiri dari tiga file yang sesuai untuk halaman utama, admin, dan login.<br />

### 4.2 Integrasi dengan HTML dan CSS

#### 4.2.1 Membuat file HTML

##### 1. Halaman utama (index.html)

Kita akan memulai dengan membuat halaman utama (index.html). Halaman ini akan menampilkan tabel sederhana namun tabel tersebut akan kita panggil atau dimuat dengan menggunakan JavaScript.<br />

![Gambar](Images/mainhtml.png) <br />

Jangan lupa untuk memanggil link CSS dan Script JavaScript-nya. Seperti pada contoh di atas, pemanggilan CSS menggunakan teks berwarna tosca dan untuk JavaScript menggunakan teks berwarna kuning.<br />

##### 2. Halaman admin (admin.html)

Halaman admin akan menampilkan tabel yang berisi data tabel yang sama seperti di halaman utama dan diformat dengan gaya yang sama juga. Di sini, kita akan belajar tentang struktur HTML untuk halaman admin. Tidak seperti halaman utama, pada halaman admin kita akan menyediakan kepala tabel nya atau tag (`<th>`) dan sisanya sama seperti halaman utama di muat dengan JavaScript. Maka pada halaman admin ini membutuhkan id untuk fungsi pada JavaScrip nya nanti.<br />

![Gambar](Images/minhtml.png) <br />

##### 3. Halaman login (login.html)

Halaman login akan memiliki form login sederhana dengan input untuk username dan password.<br />

![Gambar](Images/loghtml.png) <br />

## Chapter 5 Membuat API untuk Rute Angkot

### Merancang RESTful API dengan Golang

### CRUD Operation untuk Data Rute Angkot

### Testing API menggunakan Postman

## Chapter 6 Integrasi Frontend dan Backend

### Menghubungkan Frontend dengan API Backend

### Menggunakan Xhr/fetch untuk panggilan API

### Menampilkan data rute angkot dalam tabel
