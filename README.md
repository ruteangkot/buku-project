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

### chapter 4 Membuat Backend <br />
Sebelum kita membuat frontend kita harus membuat backend terlebih dahulu agar frontend nya bisa mendesain apa yang ada di dalam backend. Dalam pengembangan aplikasi web, pembuatan backend merupakan langkah awal yang sangat penting. Backend adalah bagian dari aplikasi yang bertanggung jawab untuk mengelola logika bisnis, penyimpanan data, dan komunikasi dengan server. Dengan backend yang kuat, data dan fungsionalitas aplikasi dapat diatur dengan baik dan aman. Pembuatan backend melibatkan penggunaan berbagai teknologi dan kerangka kerja yang memungkinkan pengembangan fitur seperti manajemen pengguna, otorisasi, penanganan permintaan, serta integrasi dengan basis data.

Dalam proyek ini, kita akan membuat backend untuk website Rute Angkot yang menyediakan informasi rute angkutan kota (angkot) bagi pengguna. Setelah backend selesai, kita akan melanjutkan dengan pengembangan frontend untuk menampilkan data-data yang telah dikelola oleh backend. Mari kita mulai dengan langkah-langkah pembuatan backend.

#### Berikut langkah-langkah untuk menghubungkan koneksi basis data mongodb <br />
Setelah menyiapkan MongoDB, langkah selanjutnya dalam pengembangan backend untuk website Rute Angkot adalah menghubungkan aplikasi backend dengan basis data tersebut. MongoDB adalah basis data NoSQL yang berbasis dokumen, yang menyimpan data dalam bentuk BSON (Binary JSON). Dalam langkah ini, kita akan membuat koneksi antara aplikasi backend dan MongoDB, serta menyiapkan skema dan model untuk data rute angkot.

Langkah pertama kalian bisa install Mongoose : 
kalian bisa masuk ke file project kalian dan masuk ke visual studio code
![Gambar](<Images/Screenshot (412).png>)<br />
setelah itu kalian bisa buka terminal di dalam visual studio code dan saat berada di terminal kalian bisa mengetik command di terminal "npm install moongose" seperti gambar dibawah ini.
![Gambar](<Images/Screenshot (413).png>)<br />
![Gambar](<Images/Screenshot (414).png>)<br />
tunggu sampai proses downlaodnya selesai, setelah selesai kalian bisa langsung membuat file di dalam folder backend dan buat file "database.js".
![Gambar](Images/Screenshot%20(418).png)<br />
lalu isi codingan didalamnya dengan codingan seperti gambar dibawah ini atau kalian bisa atur sesuka hati kalian.
![Gambar](Images/Screenshot%20(419).png)<br />




### Chapter 5 Membuat Frontend <br />

Setelah selesai membuat Backend, maka selanjutnya adalah membuat bagian Frontend agar data-data yang telah dibuat pada Backend dapat ditampilkan dan Website bisa di akses oleh pengguna.<br />
Frontend merupakan bagian pengembangan aplikasi web yang mencakup teknologi yang berinteraksi langsung dengan pengguna. Teknologi ini biasanya dikembangkan menggunakan HTML, CSS, JavaScript, dan alat desain grafis seperti Photoshop dan Fireworks. Tujuan pengembangan front-end adalah untuk menciptakan antarmuka pengguna grafis (GUI) yang memberikan pengalaman pengguna yang baik bagi pengguna akhir.(Jesús & Caballero, n.d.)<br />
Berikut langkah-langkah pembuatan Frontend untuk Website Rute Angkot.<br />

### 4.2 Integrasi dengan HTML dan CSS<br />

langkah pertama yaitu membuat folder baru untuk menampung file Frontend dengan cara klik logo folder pada Explorer.
![Gambar 13](<Images/Cuplikan layar 2024-06-04 094928.png>)
Beri nama folder tersebut.<br />
![Gambar 14](<Images/Cuplikan layar 2024-06-04 094954.png>)<br />
Kemudian buat file html pada folder tersebut yang akan digunakan sebagai page utama website ini. Html merupakan bahasa standar untuk membuat dan menyusun halaman web. HTML memungkinkan pengembang untuk menentukan struktur dari konten web dengan menggunakan elemen-elemen seperti heading, paragraf, gambar, tautan, dan lain-lain.
![Gambar](<Images/carbon(4).png>) <br />
Lalu lanjutkan isi pada bagian body nya seperti dibawah ini.
![Gambar](<Images/carbon (6).png>) <br />
Tambahkan class pada setiap tag yang dibutuhkan agar mempermudah style pada css nya nanti. Dan tambahkan juga tag Script sebagai konektor html dengan javascript nanti yang akan kita buat.<br />
Tambahkan juga Footer pada bagian bawah body agar tampilan sedikit lebih rapi.
![Gambar](<Images/carbon (7).png>) <br />

Selanjutnya agar tampilan website nya lebih cantik dan menarik, kita akan membuat file css pada folder Frontend. CSS memungkinkan pengaturan font, warna, dan ukuran teks dalam HTML. Pengguna dapat menerapkan style sheet untuk menyesuaikan tampilan halaman web.(Burkhard, 2022)
![Gambar](<Images/Cuplikan layar 2024-06-06 110827.png>) <br />

Dilanjutkan buat isi css nya seperti ini.<br />

Pertama import dulu CDN dari Framework skeleton css agar mempermudah penempatan layout, dan import juga Font google agar memberikan tampilan teks lebih menarik.
![Gambar](<Images/carbon (a).png>)<br />

Tambahkan lagi tag-tag ini untuk style elemen-elemen utama pada html.
![Gambar](<Images/carbon (b).png>)<br />

Karena website kita berupa tabel dan diimpor dari file javascript, maka kita tambahkan tag-tag untuk style tabel nya dan style container untuk data tabel nya.
![Gambar](<Images/carbon (c).png>)<br />

Agar tampilan nya menyesuaikan mode gelap atau tidak nya browser yang digunakan user, maka kita akan membuat query darkmode seperti ini.
![Gambar](<Images/carbon (d).png>)<br />

Selanjutnya kita akan membuat query agar tampilan website kita dapat dibuka pada tampilan mobile tanpa merusak layout yang sudah dibuat.
![Gambar](<Images/carbon (e).png>)<br />

Setelah css selesai, sekarang lanjut membuat file javascript agar semua fungsi yang ada dapat di gunakan. JavaScript dapat digunakan untuk memanipulasi konten, mengontrol multimedia, menganalisis data, dan banyak lagi. Tambahkan lagi file baru javascript.
![Gambar](<Images/Cuplikan layar 2024-06-06 110920.png>) <br />

Lanjutkan isi file javascript nya. Tambahkan fungsi ini agar data dari Backend dapat dimuat pada Frontend.
![Gambar](<Images/carbon (g).png>)<br />

Karena data merupakan data tabel, maka selanjutnya adalah membuat fungsi agar data yang dimuat langsung berbentuk tabel.
![Gambar](<Images/carbon (h).png>)<br />

Lalu terkahir kita akan membuat fungsi untuk placeholder agar kolom input pencarian rute dapat bergfungsi.
![Gambar](<Images/carbon (i).png>)<br />

Selanjutnya membuat folder admin untuk page admin. Buat folder lagi seperti awal membuat file Frontend<br />

Buat file html, css, dan javascript seperti awal.<br />
![Gambar](Images/)<br />

Isi file html nya seperti awal html utama.<br />
![Gambar](<Images/carbon (k).png>)<br />

Lanjut isi file css agar tampilan nya seperti css utama.<br />
![Gambar](<Images/carbon%20(l).png>)<br />

Dan terakhir isi file javascript nya. Pada file javascript ini seperti file javascript utama, namun ada beberapa tambahan code untuk fungsi CRUD.<br />
![Gambar](<Images/carbon%20(l).png>)<br />

Tambahkan fungsi-fungsi ini untuk menjalankan CRUD
![Gambar](<Images/carbon%20(o).png>)<br />

## Chapter 5 Membuat API untuk Rute Angkot

### Merancang RESTful API dengan Golang

### CRUD Operation untuk Data Rute Angkot

### Testing API menggunakan Postman

## Chapter 6 Integrasi Frontend dan Backend

### Menghubungkan Frontend dengan API Backend

### Menggunakan Xhr/fetch untuk panggilan API

### Menampilkan data rute angkot dalam tabel
