# Website Rute Angkot

## Chapter 1 Pengenalan Website Rute Angkot<br />

### 1.1 APA ITU WEBSITE RUTE ANGKOT<br />

Website rute angkot adalah platform digital yang menyediakan informasi tentang rute angkutan kota (angkot) dalam bentuk tabel. Website ini memungkinkan pengguna untuk mencari dan menampilkan rute angkot yang tersedia di suatu kota, serta memberikan informasi detail mengenai jalur yang dilalui dan titik pemberhentian.<br />

### 1.2 Tujuan dan Manfaat Website Rute Angkot<br />

Dengan adanya website rute angkot, masyarakat dapat dengan mudah menemukan rute angkot yang mereka butuhkan, mengurangi ketergantungan pada informasi manual, dan meningkatkan efisiensi dalam penggunaan angkutan umum. Platform ini juga dapat membantu pemerintah dan operator angkutan kota dalam mengelola dan mengoptimalkan rute angkot.

## Chapter 2 Pengenalan Teknologi<br />

#### 2.1.2 BACKEND<br />

“Backend” mewakili elemen sisi server dalam kerangka web yang berfungsi sebagai mediator antara klien dan repositori data, seperti database, cache Redis, atau penyimpanan blob. Ini bertanggung jawab untuk mengelola logika operasional, manipulasi data, dan komunikasi dengan database atau aset tambahan yang penting untuk mendukung aplikasi berbasis web.(Morozov, 2020)<br />

#### 2.1.6 Visual Studio Code<br />

Visual Studio Code adalah editor kode sumber terbuka oleh Microsoft. Visual Studio Code mendukung berbagai bahasa pemrograman dan dikenal untuk fitur seperti debugging dan penyelesaian kode. Biasanya digunakan untuk pengembangan web dan berbasis cloud, berkat fleksibilitas dan perpustakaan ekstensinya. Editor menawarkan kontrol, manajemen build, pengujian unit, dan kemampuan pengujian statis. Dengan fitur-fitur ini, menjadikannya alat yang berharga bagi pengembang.(Murari & Sandru, 2013)

#### 2.1.7 MongoDB <br />

MongoDB adalah database NoSQL yang menggunakan model dokumen, yang berarti data disimpan dalam format JSON-like yang fleksibel. MongoDB sangat cocok untuk aplikasi yang memerlukan skema dinamis dan dapat menangani berbagai jenis data. Keunggulan MongoDB termasuk skalabilitas yang mudah, performa tinggi, dan kemampuan untuk menangani data yang besar. Berikut adalah contoh dokumen MongoDB:
![Gambar](<Images/carbon(7).png>) <br />

![Gambar](<Images/carbon(8).png>) <br />

## Chapter 3 Pengenalan Database dan Penginstall-an MongoDB <br />

### Pengenalan Database <br />

Apa itu Database?
Database adalah kumpulan data yang disusun secara sistematis agar dapat diakses, dikelola, dan diperbarui dengan mudah. Database memungkinkan penyimpanan data dalam jumlah besar dengan cara yang terstruktur sehingga dapat digunakan untuk berbagai keperluan, seperti analisis data, pengambilan keputusan, dan penyimpanan informasi penting. <br />

#### Penginstall-an MongoDB <br />

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

### Chapter 5 Membuat Frontend <br />

Setelah selesai membuat Backend, maka selanjutnya adalah membuat bagian Frontend agar data-data yang telah dibuat pada Backend dapat ditampilkan dan Website bisa di akses oleh pengguna.<br />
Frontend merupakan bagian pengembangan aplikasi web yang mencakup teknologi yang berinteraksi langsung dengan pengguna. Teknologi ini biasanya dikembangkan menggunakan HTML, CSS, JavaScript, dan alat desain grafis seperti Photoshop dan Fireworks. Tujuan pengembangan front-end adalah untuk menciptakan antarmuka pengguna grafis (GUI) yang memberikan pengalaman pengguna yang baik bagi pengguna akhir.(Jesús & Caballero, n.d.)<br />
Berikut langkah-langkah pembuatan Frontend untuk Website Rute Angkot.<br />

#### Berikut langkah-langkah pembuatan Frontend untuk Website Rute Angkot.<br />

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
