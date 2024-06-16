# Pengembangan Website Rute Angkot

## KATA PENGANTAR

Segala puji dan syukur kami panjatkan kepada Tuhan Yang Maha Esa atas limpahan rahmat dan karunia-Nya sehingga buku ini dapat diselesaikan dengan baik. Salawat serta salam semoga selalu tercurah kepada Nabi Besar Muhammad SAW.<br />

Kami ingin mengucapkan terima kasih yang sebesar-besarnya kepada semua pihak yang telah memberikan dukungan dan bantuan dalam penulisan buku ini, mulai dari orang tua, dosen pembimbing, rekan-rekan, hingga semua pihak yang tidak dapat kami sebutkan satu per satu.<br />

Buku ini, yang berjudul "Pengembangan Website Rute Angkot", dibuat dengan harapan dapat memberikan panduan praktis bagi pembaca dalam mengembangkan aplikasi atau sistem terkait. Kami berusaha sebaik mungkin untuk menyajikan isi buku ini dengan lengkap dan mudah dipahami.<br />

Kami menyadari bahwa buku ini masih jauh dari sempurna. Oleh karena itu, kritik dan saran yang membangun dari para pembaca sangat kami harapkan untuk perbaikan di masa mendatang.<br />

Semoga buku ini dapat bermanfaat dan menambah wawasan bagi para pembaca dalam bidang pengembangan website, serta memberikan kontribusi positif bagi masyarakat. Terima kasih.<br />

## PRAKATA

Di era digital yang terus berkembang pesat, teknologi telah menyentuh berbagai aspek kehidupan, termasuk transportasi. Angkutan kota (angkot) memiliki peran vital dalam kehidupan masyarakat perkotaan, dan kini informasi rute angkot dapat diakses dengan mudah melalui internet.

Website rute angkot adalah salah satu teknologi yang semakin diminati, karena memudahkan pengguna untuk mengakses informasi mengenai rute, jadwal, dan detail lainnya dengan cara yang terstruktur dan mudah diakses. Pembuatan website yang menampilkan tabel rute angkot menjadi sangat penting, karena memungkinkan pengguna memperoleh informasi dengan cepat dan tepat.

Buku ini bertujuan untuk memberikan panduan yang komprehensif tentang cara merancang dan membangun website yang menampilkan tabel rute angkot. Setiap chapter dalam buku ini disusun dengan langkah-langkah yang mudah diikuti, khususnya bagi pembaca yang baru memulai.

Kami berharap buku ini dapat memberikan kontribusi positif dalam meningkatkan keterampilan pengembangan website para pembaca. Terima kasih telah memilih buku ini sebagai panduan belajar Anda.

Selamat belajar dan semoga sukses!

## DAFTAR ISI

### CHAPTER 1 PENGENALAN GOLANG DAN JAVASCRIPT

#### 1.1 DEFINISI GOLANG

#### 1.2 DEFINISI JAVASCRIPT

#### 1.3 KELEBIHAN MENGGUNAKAN GOLANG DAN JAVASCRIPT DALAM PENGEMBANGAN WEB

### CHAPTER 2 PERSIAPAN LINGKUNGAN PENGEMBANG

#### 2.1 CARA INSTALASI GOLANG

#### 2.2 SETTING UP VISUAL STUDIO CODE DAN EKTENSI YANG DIPERLUKAN

### CHAPTER 3 MEMBANGUN BACKEND DENGAN GOLANG

#### 3.1 STRUKTUR DASARA PROYEK GOLANG

#### 3.2 MENGHUBUNGKAN KE DATABASE (MONGODB)

### CHAPTER 4 MEMBANGUN FRONTEND DENGAN JAVASCRIPT

#### 4.1 STRUKTUR DASAR PROYEK JAVASCRIPT

#### 4.2 INTEGRASI HTML DAN CSS

### CHATER 5 MEMBUAT API RUTE ANGKOT

#### 5.1 MERANCANG RESTFUL API DENGAN GOLANG

#### 5.2 CRUD OPERATION UNTUK DATA RUTE ANGKOT

#### 5.3 TESTING API MENGGUNAKAN POSTMAN

### CHAPTER 6 INTEGRASI FRONTEND DAN BACKEND

#### 6.1 MENGHUBUNGKAN FRONTEND DENGAN API BACKEND

### CHAPTER 7 MENAMPILKAN UI WEBSITE YANG SUDAH DIBUAT

#### 7.1 TAMPILAN USER

#### 7.2 TAMPILAN ADMIN

### DAFTAR PUSTAKA

### TENTANG PENULIS

## CHAPTER 1 PENGENALAN GOLANG DAN JAVASCRIPT<br />

### 1.1 DEFINISI GOLANG<br />

Go, juga dikenal sebagai Golang, adalah bahasa pemrograman yang dikembangkan oleh Google untuk membantu Anda menulis kode secara efisien dan mudah, aman, terukur, dan mudah dipelihara. Go dirancang untuk menyederhanakan manajemen ketergantungan dan proses pengembangan perangkat lunak. Bahasa ini secara asli mendukung konkurensi dan konkurensi, menjadikannya pilihan populer untuk pengembangan perangkat lunak yang memerlukan kinerja dan skalabilitas tinggi.(Blumen & Meyerson, n.d.)<br />

### 1.2 DEFINISI JAVASCRIPT<br />

JavaScript, bahasa pemrograman skrip yang banyak digunakan, memegang posisi penting dalam lanskap aplikasi web kontemporer. Bahasa ini, yang dicirikan oleh sifatnya yang dinamis, sistem pengetikan longgar, dan properti asinkron, mengambil peran penting dalam mengaktifkan fungsionalitas interaktif dalam platform berbasis web. Selain itu, JavaScript digunakan secara luas untuk memfasilitasi manipulasi real-time dan interaksi dengan Document Object Model (DOM), komponen penting dalam struktur halaman web.(Ocariza et al., 2015)<br />

### 1.3 KELEBIHAN MENGGUNAKAN GOLANG DAN JAVASCRIPT DALAM PENGEMBANGAN WEB

#### KELEBIHAN GOLANG (GO)

1. Golang memiliki performa yang sangat baik karena dikompilasi menjadi kode mesin, sehingga berjalan lebih cepat dibandingkan bahasa yang diinterpretasikan seperti JavaScript.<br />
2. Golang memiliki dukungan bawaan yang sangat kuat untuk concurrency melalui goroutines dan channels, yang memudahkan pengembangan aplikasi dengan kemampuan pemrosesan paralel yang efisien.<br />
3. Golang adalah bahasa yang statically written, yang berarti banyak kesalahan bisa ditangkap pada saat kompilasi, sehingga mengurangi bug pada runtime.<br />
4. Sintaks Golang dirancang untuk sederhana dan mudah dibaca, yang membuatnya lebih mudah untuk dipelajari dan dipahami.<br />
5. Waktu kompilasi Golang sangat cepat dibandingkan dengan banyak bahasa lain yang dikompilasi, yang mempercepat siklus pengembangan.<br />
6. Golang memiliki ekosistem yang kuat dengan banyak pustaka dan alat bantu, serta komunitas yang aktif.<br />

#### KELEBIHAN JAVASCRIPT

1. JavaScript adalah bahasa pemrograman yang withering umum digunakan untuk pengembangan front-end web. Semua browser cutting edge mendukung JavaScript, membuatnya esensial untuk pengembangan aplikasi web interaktif.<br />
2. JavaScript memiliki ekosistem yang sangat luas dengan banyak system dan library populer seperti Respond, Precise, dan Vue.js untuk pengembangan front-end, serta Node.js untuk back-end.<br />
3. JavaScript memiliki dukungan kuat untuk offbeat programming dengan fitur seperti Guarantees, async/await, dan event-driven programming, yang penting untuk pengembangan aplikasi web present day yang responsif.<br />
4. JavaScript memiliki komunitas pengembang yang sangat besar dan aktif, yang menyediakan banyak sumber daya, instructional exercise, dan alat bantu untuk pengembangan web.<br />
5. JavaScript memungkinkan pembuatan aplikasi web yang dapat memperbarui konten secara real-time tanpa perlu memuat ulang halaman, berkat teknologi seperti WebSockets dan system seperti Meteor.js.<br />

## CHAPTER 2 PERSIAPAN LINGKUNGAN PENGEMBANG<br />

### 2.1 CARA INSTALASI GOLANG<br />

Golang, atau Go, adalah bahasa pemrograman yang dikembangkan oleh Google. Go dirancang untuk efisiensi, kemudahan penggunaan, dan kecepatan kompilasi. Bahasa ini memiliki fitur seperti pengelolaan memori otomatis, tipe data statis, dan dukungan concurrency yang kuat, menjadikannya pilihan yang baik untuk pengembangan aplikasi yang skalabel dan cepat.<br />

Berikut adalah cara singkat untuk menginstal Golang di berbagai sistem operasi:

#### Instalasi di Windows <br />

1. Unduh installer Golang: caranya dengan mengunjungi website Golang kalian bisa mengetik di kolom pencarian browser kalian "Golang" dan kalian akan di alihkan ke website seperti gambar dibawah ini.
   [GambarinstalasiGolang](<Images/Screenshot (457).png>)<br />

### 2.2 SETTING UP VISUAL STUDIO CODE DAN EKSTENSI YANG DIPERLUKAN<br />

Visual Studio Code adalah editor kode sumber terbuka oleh Microsoft. Visual Studio Code mendukung berbagai bahasa pemrograman dan dikenal untuk fitur seperti debugging dan penyelesaian kode. Biasanya digunakan untuk pengembangan web dan berbasis cloud, berkat fleksibilitas dan perpustakaan ekstensinya. Editor menawarkan kontrol, manajemen build, pengujian unit, dan kemampuan pengujian statis. Dengan fitur-fitur ini, menjadikannya alat yang berharga bagi pengembang.(Murari & Sandru, 2013)

## CHAPTER 3 MEMBANGUN BACKEND DENGAN GOLANG <br />

“Backend” mewakili elemen sisi server dalam kerangka web yang berfungsi sebagai mediator antara klien dan repositori data, seperti database, cache Redis, atau penyimpanan blob. Ini bertanggung jawab untuk mengelola logika operasional, manipulasi data, dan komunikasi dengan database atau aset tambahan yang penting untuk mendukung aplikasi berbasis web.(Morozov, 2020)<br />

### 3.1 STRUKTUR DASAR PROYEK GOLANG<br />

[GambarStrukturProjekGolang](<Images/Screenshot (459).png>)<br />

#### Penjelasan Bagian Folder <br />

1. github/: Berisi konfigurasi untuk GitHub, seperti workflow untuk GitHub Actions.
2. config/: Biasanya digunakan untuk menyimpan file konfigurasi aplikasi, seperti file konfigurasi database atau environment variables.
3. controller/: Menyimpan logika untuk menangani permintaan HTTP. Controller berisi fungsi yang akan dipanggil oleh route.
4. helper/: Berisi fungsi utilitas atau helper yang dapat digunakan di berbagai bagian aplikasi.
5. model/: Menyimpan definisi struktur data atau model yang digunakan dalam aplikasi, biasanya berhubungan dengan database.
6. route/: Berisi definisi rute untuk aplikasi web, menentukan endpoint dan controller mana yang harus dipanggil.<br />

##### Penjelasan Bagian File <br />

1. gcloudignore: Berisi daftar file atau direktori yang akan diabaikan saat melakukan deployment ke Google Cloud.
2. gitignore: Berisi daftar file atau direktori yang akan diabaikan oleh Git.
3. go.mod: Berisi informasi modul Go, seperti nama modul dan dependensi yang digunakan.
4. go.sum: Berisi checksum dari dependensi yang digunakan, memastikan integritas dependensi.
5. LICENSE: Berisi informasi lisensi proyek.
6. main.go: File utama aplikasi Go yang biasanya berisi titik masuk utama (main function) dari aplikasi.
7. README.md: Berisi dokumentasi proyek, penjelasan tentang cara instalasi, penggunaan, dan informasi lainnya yang relevan.<br />

### 3.2 MENGHUBUNGKAN KE DATABASE (MongoDB) <br />

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

## CHAPTER 4 MEMBANGUN FRONTEND DENGAN JAVASCRIPT <br />

### 4.1 STRUKTUR DASAR PROYEK JAVASCRIPT

![Gambar](Images/directory%20front.png) <br />

Pada bagian Frontend, struktur direktori bisa disesuaikan sesuai keinginan. Namun, yang paling penting adalah dalam struktur ini terdapat tiga file HTML: satu untuk halaman utama, satu untuk halaman admin, dan satu untuk halaman login. Demikian juga dengan file CSS dan JavaScript, masing-masing terdiri dari tiga file yang sesuai untuk halaman utama, admin, dan login.<br />

### 4.2 INTEGRASIKAN HTML DAN CSS

#### 4.2.1 MEMBUAT FILE HTML

##### 1. HALAMAN UTAMA (index.html)

Kita akan memulai dengan membuat halaman utama (index.html). Halaman ini akan menampilkan tabel sederhana namun tabel tersebut akan kita panggil atau dimuat dengan menggunakan JavaScript.<br />

![Gambar](Images/mainhtml.png) <br />

Jangan lupa untuk memanggil link CSS dan Script JavaScript-nya. Seperti pada contoh di atas, pemanggilan CSS menggunakan teks berwarna tosca dan untuk JavaScript menggunakan teks berwarna kuning.<br />

##### 2. HALAMAN ADMIN (admin.html)

Halaman admin akan menampilkan tabel yang berisi data tabel yang sama seperti di halaman utama dan diformat dengan gaya yang sama juga. Di sini, kita akan belajar tentang struktur HTML untuk halaman admin. Tidak seperti halaman utama, pada halaman admin kita akan menyediakan kepala tabel nya atau tag (`<th>`) dan sisanya sama seperti halaman utama di muat dengan JavaScript. Maka pada halaman admin ini membutuhkan id untuk fungsi pada JavaScrip nya nanti.<br />

![Gambar](Images/minhtml.png) <br />

##### 3. HALAMAN LOGIN (login.html)

Halaman login akan memiliki form login sederhana dengan input untuk username dan password.<br />

![Gambar](Images/loghtml.png) <br />

#### 4.2.2 MENGINTEGRASIKAN CSS

##### 1. GAYA UMUM (style.css)

Kita akan membuat file CSS untuk halaman utama yang akan mengatur tampilan umum tabel dan elemen lain di halaman utama. Anda akan belajar tentang dasar-dasar CSS dan bagaimana menggunakannya untuk membuat halaman web terlihat lebih menarik.<br />
Ini kode yang mengatur elemen utama pada html. Dan yang mengatur image jika anda menambahkan gambar pada html anda.<br />

![Gambar](Images/cssutama1.png) <br />

![Gambar](Images/cssutama2.png) <br />

Pada bagian ini merupakan bagian yang mengatur gaya pada tabel.<br />

![Gambar](Images/cssutama3.png) <br />

Dan pada bagian ini untuk mengatur gaya pada footer nya.<br />

![Gambar](Images/cssutama4.png)<br>

Jangan lupa import CDN untuk framework CSS Skeleton untuk layout yang lebih rapih. Dan import font dari google, untuk font bisa disesuaikan sesuai keinginan. <br />

![Gambar](Images/cssimport.png)<br />

Tambahkan juga media query agar tampilan dapat di buka pada perangkat mobile dan tetap menjaga kerapihan semua layout nya.<br />

![Gambar](Images/cssresponsive.png) <br />

Terakhir tambahkan juga query untuk menyesuaikan warna pada semua elemen nya jika browser menggunakan dark mode atau tidak. Ini opsional tergantung keinginan.<br />

![Gambar](Images/cssdarkmode.png) <br />

##### 2. GAYA KHUSUS HALAMAN ADMIN (admin/admin.html)

Kita akan membuat file CSS khusus untuk halaman admin, memberikan gaya yang sedikit berbeda untuk tabel dan elemen lainnya. Ini menunjukkan bagaimana kita bisa memiliki gaya khusus untuk halaman yang berbeda dalam proyek yang sama.<br />

Karena banyak nya elemen pada halaman admin, ini menjadikan kode nya lebih banyak daripada CSS halaman utama. Banyak elemen yang harus di style pada halaman ini. Berikut kode nya. <br />

Pertama import juga font google dan CDN untuk Framework CSS Skeleton nya seperti pada CSS utama.<br />

Lanjut isi kode-kode ini.<br />

![Gambar](Images/cssadmin1.png)<br />

Karena pada halaman ini memang memiliki banyak elemen, terutama elemen modal yang digunakan pada javascript nya untuk menangani suatu fungsi. Maka dari itu kita akan memberikan gaya yang sesuai untuk modal tersebut.<br />

![Gambar](Images/cssadmin2.png)<br />

Dan jangan lupa tambahkan juga kode untuk query responsive nya.<br />

![Gambar](Images/cssadmin4.png)<br />

Tamabahkan juga kode untuk query mode gelap nya seperti pada CSS utama jika memang membutuhkan.<br >

##### 3. GAYA KHUSUS HALAMAN LOGIN (login/login.html)

Nahh, terakhir gaya untuk file CSS halaman login. Pada file ini akan fokus pada penataan form login agar terlihat lebih rapi dan profesional.<br />

Seperti pada file CSS sebelumnya import font google dan Framework CSS Skeleton.<br />
Lanjut isi kode nya seperti ini.<br />

![Gambar](Images/csslogin1.png)<br />

Pada halaman login ini tidak terlalu banyak elemen yang dibuat, maka pada pembuatan query responsive nya juga tidak terlalu banyak.<br />

![Gambar](Images/csslogin2.png)<br />

### 4.3 INTEGRARSI JAVASCRIPT

#### MEMBUAT FILE JAVASCRIPT

##### 1. SKRIP UTAMA (javascript/main.js)

Kita akan membuat file JavaScript untuk halaman utama. Skrip ini akan menambahkan interaktivitas ke tabel atau elemen lainnya di halaman utama. Anda akan belajar tentang event handling dan manipulasi DOM dengan JavaScript.<br />

Agar data nya di muat sesuai dengan tag (`<th>`) yang pada HTML atau data nya dapat masuk ke dalam tabel, maka perlu dibuat fungsi seperti dibawah ini.<br />

![Gambar](Images/mainjs1.png)<br />

Selanjutnya, untuk membuat kolom pencarian rute nya dapat berjalan dibutuhkan fungsi seperti ini.<br />

![Gambar](Images/mainjs2.png)<br />

##### 2. SKRIP ADMIN (admin/admin.js)

File JavaScript untuk halaman admin akan mengandung skrip yang dibutuhkan untuk fungsi-fungsi admin, seperti manipulasi data tabel. Ini menunjukkan bagaimana kita bisa menambahkan fungsionalitas yang berbeda di halaman admin.<br />

Sama seperti file javascript utama, kita akan buat fungsi agar data nya masuk ke dalam tabel, namun sedikit berbeda dengan file javascript utama. Ada penambahan elemen lain pada file javascript ini.<br />

![Gambar](Images/adminjs1.png)<br />

Seperti yang sudah kita singgung pada pembahasan CSS sebelum nya mengenai modal, disinilah kita akan membuat modal tersebut. Berikut kode nya.<br />

![Gambar](Images/adminjs2.png)<br />

##### 3. SKRIP LOGIN (login/login.js)

File JavaScript untuk halaman login akan mengandung skrip yang berfungsi untuk validasi form atau fungsi lain yang diperlukan untuk halaman login. Ini akan membantu meningkatkan keamanan dan pengalaman pengguna di halaman login.<br />

Untuk file javascript login tidak terlalu banyak fungsi dan kode yang dibuat, tapi sementara buat kode nya seperti dulu.<br />

![Gambar](Images/loginjs.png)<br />

## CHAPTER 5 MEMBUAT API UNTUK RUTE ANGKOT

### 5.1 MERANCANG RESTFUL API DENGAN GOLANG

### 5.2 CRUD OPERATION UNTUK DATA RUTE ANGKOT

### 5.3 TESTING API MENGGUNAKAN POSTMAN

## CHAPTER 6 INTEGRASI FRONTEND DAN BACKEND

### 6.1 MENGHUBUNGKAN FRONTNEND DENGAN API BACKEND

## CHAPTER 7 TAMPILAN UI WEBSITE YANG SUDAH DIBUAT

### 7.1 TAMPILAN USER

### 7.2 TAMPILAN ADMIN

## DAFTAR PUSTAKA

## TENTANG PENULIS
