# ECOWASTEWATER

Platfrom sanitasi ini digunakan untuk mempermudah masyarakat dalam melaporkan permasalahan air limbah langsung ke pihak terkait, dan juga dapat membantu masyarakat memahami pentingnya menjaga sanitasi melalui action, laporan dapat dibuat dengan cepat dan tepat, serta melalui community yang memperkuat kerja sama antara masyarakat dan instansi agar penanganan air limbah lebih efektif dan lingkungan tetap terjaga.

** EcowasteWater 
EcowasteWater merupakan patform yang berfungsi sebagai sistem digital untuk mempermudah pengelolaan sanitasi dan air limbah melalui pemantauan, pelaporan, dan penyimpanan data secara terpusat. Melalui platform ini, masyarakat dapat melaporkan permasalahan terkait fasilitas sanitasi atau air limbah dengan cepat, sementara pihak pengelola dapat langsung menerima laporan, memverifikasi kondisi di lapangan, dan menindaklanjutinya sesuai prioritas. Sistem ini juga menyimpan data inspeksi, kondisi instalasi, dan riwayat perawatan secara otomatis, sehingga proses evaluasi dan pengambilan keputusan menjadi lebih akurat dan efisien.

## Fitur

### OOP
Object Oriented Programming (OOP) merupakan fondasi dalam pengembangan aplikasi karena memungkinkan proses pemrograman dilakukan dengan cara yang lebih terstruktur, terorganisir, dan mudah dikembangkan.


### Encapsulation
Encapsulation merupakan konsep dalam Object Oriented Programming (OOP) yang bertujuan untuk menggabungkan data dengan fungsi yang mengelolanya dalam satu kesatuan (Class), serta membatasi akses langsung ke data tersebut. Dengan cara ini, data menjadi lebih terkontrol dan terproteksi karena hanya dapat diakses melalui method yang telah disediakan.


### Abstraction
berfokus pada penyederhanaan kompleksitas dengan hanya menampilkan bagian penting dari suatu objek dan menyembunyikan detail yang tidak diperlukan. Dengan abstraction, jadi hanya memberikan informasi atau fungsi yang relevan untuk digunakan.


### Inheritance
Inheritance merupakan konsep yang memungkinkan suatu class mewarisi sifat (atribut) dan perilaku (method) dari class lain. Class yang mewarisi disebut subclass, sedangkan class yang memberikan warisan disebut parent superclass. Dengan inheritance, maka tidak perlu menulis ulang kode yang sama, karena subclass dapat menggunakan atau mengembangkan fitur yang sudah ada pada superclass.


### Polymorphism
Polymorphism adalah konsep yang memungkinkan satu nama method digunakan oleh beberapa class dengan cara atau hasil yang berbeda. Dengan adanya polymorphism, objek yang berbeda dapat merespons atau menjalankan perintah yang sama, tetapi dengan cara yang sesuai dengan karakteristik masing-masing.


### Interface 
Interface merupakan struktur yang berisi kumpulan method tanpa implementasi (hanya berupa deklarasi). Interface berfungsi sebagai kontrak atau perjanjian yang harus dipatuhi oleh class yang menggunakannya. 


## Packages
Packages berfungsi mengelompokkan class dan file-file program lainnya ke dalam satu wadah atau folder tertentu. Dengan adanya package, struktur program menjadi lebih teratur, mudah dikelola, serta menghindari konflik nama class yang sama.

<img width="426" height="245" alt="image" src="https://github.com/user-attachments/assets/d5c61a63-8618-45e4-b83b-3e93f7dd8feb" />

### Icon
Package icon diguanakn untuk menyimpan file-file ikon atau gambar, dengan adanya package icon, file tidak akan bercampur dengan class java, sehingga struktur project lebih rapi dan terorganisir.

<img width="411" height="514" alt="image" src="https://github.com/user-attachments/assets/61be8624-d6cc-48f3-8144-513142e92e20" />


### Koneksi
Package koneksi berfungsi untuk tempat mengelola semua file yang berkaitan dengan koneksi ke database. Terdapat dua file yaitu DatabaseConfig.java yang berfungsi untuk menghubungkan aplikasi ke database seperti MySQL. Kemudian ada file TesKoneksi.java yang berfungsi untuk memastikan bahwa database dapat di akses sebelum aplikasi di gunakan.

<img width="416" height="80" alt="image" src="https://github.com/user-attachments/assets/0dd1f51f-342d-427c-8093-02552278d7c7" />


### Main
Package Main berfungsi sebagai pusat logika, yaitu tempat menyimpan semua class yang terkait dengan proses uatama atau tampilan program.

<img width="408" height="487" alt="image" src="https://github.com/user-attachments/assets/c64d170a-402e-47af-adec-b3bbc249235b" />

### File untuk Admin yang di awali huruf "A"
* A_Edit_Status.java : Form/class untuk admin dalam mengedit status laporan air limbah.
* A_Hapus_Laporan.java : Digunakan admin untuk menghapus laporan dari sistem.
* A_Lihat_Laporan.java : Admin dapat melihat daftar laporan yang masuk.
* A_Register_Petugas.java : Admin mendaftarkan akun petugas baru.
* A_Welcome.java : Halaman sambutan / dashboard awal untuk admin.
* A_update_data_petugas.java : Admin memperbarui data profil petugas.

### File untuk Masyarakat yang di awali dengan huruf "M"
* M_Buat_Laporan.java : Form untuk masyarakat membuat laporan masalah sanitasi/limbah.
* M_Lihat_Laporan.java : Masyarakat dapat melihat status laporan yang pernah dikirim.
* M_Welcome.java : Halaman sambutan / dashboard untuk masyarakat.

### File untuk Petugas yang diawali huruf "P"
* P_Edit_Status.java : Petugas mengubah status laporan (ditangani, selesai, dll.).
* P_Lihat_Laporan.java : Petugas melihat daftar laporan yang harus ditangani.
* P_Tindak_Lanjut.java : Form untuk mengisi tindakan lanjutan setelah menangani laporan.
* P_Welcome.java : Dashboard/halaman awal petugas.

### Halaman Umum
* Landing_Page.java : Tampilan awal aplikasi sebelum login.
* Login.java : Form login untuk admin, petugas, dan masyarakat.
* Register_Masyarakat.java : Halaman registrasi untuk masyarakat.
* PA_SanitasiAirLimbah.java : Kemungkinan merupakan halaman utama yang menampilkan fitur aplikasi atau modul sanitasi (PA = Project Application / aplikasi utama).


## Dependencies, Java Dependencies, dan Project Files

### Dependencies 
* AbsoluteLayout-RELEASE270.jar : Library layout bawaan NetBeans untuk mengatur posisi komponen secara bebas (AbsoluteLayout). Biasanya dipakai saat design GUI di NetBeans.
* mysql-connector-j-9.4.0.jar : Driver koneksi ke database MySQL/MariaDB. Tanpa file ini aplikasi tidak bisa melakukan connect, INSERT, SELECT, UPDATE, dll ke MySQL.
* protobuf-java-4.31.1.jar : Library Google Protocol Buffers. Biasanya dipakai oleh MySQL Connector versi baru untuk komunikasi atau serialisasi data.

### Java Dependencies
* JDK 24 (Default) : Artinya project menggunakan Java Development Kit versi 24 sebagai compiler dan runtime.

### Project Files
* Berisi struktur file utama project (source code .java, form .form, dan package lainnya).


## Flowchart & Use Case

Berikut adalah link Flowchart dan Use case diagram 

Flowchart : https://app.diagrams.net/#G1wKB05q0JbQ4xsn0khmI7zLCrlHOijzv4#%7B%22pageId%22%3A%2280WTy4hSo2W5AGeVKFtQ%22%7D

Use case : https://app.diagrams.net/#G1zMjbFOPNwCFiWQZRNhJr3RCdtqx2eVic#%7B%22pageId%22%3A%22AUcS-lJaB4qKYF_lkGg9%22%7D


## grapgical User Interface (GUI)

### Halaman Landing Page
Merupakan halaman utama ketika pertama kali masuk ke platfrom. 

### Halaman Login 
Merupakan halaman setelah landing page, dengan fitur role, login sebagai admin, petugas, dan masyarakat, serta fitur registrasi untuk masyarakat

## Admin

### Halaman Wellcome 
Merupakan halaman setelah login sebagai Admin dengan fitur lihat laporan, dan ada beberapa fitur yang hanya bisa di akses oleh admin seperti hapus laporan, registrasi petugas, ubah status, dan edit data petugas.

### Halaman Lihat Laporan
Merupakan halaman ketika admin memilih fitur lihat laporan yang menampilkan seluruh laporan baik yang sudah di tangani dan yang sedang di peroses

### Halaman Hapus laporan
Merupakan halaman ketika admin memilih fitur hapus laporan yang menampilkan seluruh laporan dan dapat di hapus

### halaman Registrasi Petugas
Merupakan halaman ketika admin memilih fitur registrasi petugas yang menampilkan dan menginput nama lengkap, username, password, no telepon, dan wilayah penugasan. Jadi akun petugas hanya di registrasikan oleh admin, bukan di petugas.

### Hamana Ubah Status
Merubahakan halaman ketika admin memilih fitur ubah status yang menampilkan seluruh laporan dan memilih laporan mana yang ingin di ubah ststusnya seperti, sedang di proses atau sudah di tangani.

### Halaman Edit data Petugas
Merupakan hamana ketika admin memilih fitur edit data petugas yang menampilkan halaman seperti registrasi petugas, dan admin dapat merubah data petugas tertentu.


## Petugas

### Halaman Wellcome 
Merupakan haman ketika login sebagai petugas dengan menampilkan fitur lihat laporan, ubah status, dan tindak lanjut.

### Halaman Lihat Laporan
Merupakan halaman ketika petugas memilih fitur lihat laporan dan menampilkan seluruh laporan baik yang belum di tangani dan sudah di tangani.

### Halaman Ubah Status
Merupakan halaman ketika petugas memilih fitur uabh status yang menampilkan seluruh laporan dan dapat mengedit status laporan baik belum di tangani dan sudah di tangani

### halaman Tindak lanjut
Merupakan halaman ketika petugas memilih fitur tindak lanjut yang menampilkan tanggal tindakan, foto, dan keteranga, setelah menangai laporan.


## Masyarakat

### Halaman Registrasi Masyarakat
Merupakan haman ketika pengguna belum memiliki akun dengan menampilkan inputan nama, username, password, no telepon, dan alamat.

### Halaman Wellcome 
Merupakan halaman ketika login sebagai masyarkat dengan menampilkan fitur buat laporan, dan lihat laporan.

### Halaman Buat Laporan
Menampilkan halaman ketika pengguna memilih fitur buat laporan dengan menampilkan inputan nama lengkap, wilayah, layanan, foto, dan tanggal laporan.

### halaman Lihat Laporan
Menampilkan halaman ketika pengguna memilih fitur lihat laporan yang sudah di buat sebelumnya



