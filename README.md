# ECOWASTEWATER

Platfrom sanitasi ini digunakan untuk mempermudah masyarakat dalam melaporkan permasalahan air limbah langsung ke pihak terkait, dan juga dapat membantu masyarakat memahami pentingnya menjaga sanitasi melalui action, laporan dapat dibuat dengan cepat dan tepat, serta melalui community yang memperkuat kerja sama antara masyarakat dan instansi agar penanganan air limbah lebih efektif dan lingkungan tetap terjaga.

## EcowasteWater 
EcowasteWater merupakan patform yang berfungsi sebagai sistem digital untuk mempermudah pengelolaan sanitasi dan air limbah melalui pemantauan, pelaporan, dan penyimpanan data secara terpusat. Melalui platform ini, masyarakat dapat melaporkan permasalahan terkait fasilitas sanitasi atau air limbah dengan cepat, sementara pihak pengelola dapat langsung menerima laporan, memverifikasi kondisi di lapangan, dan menindaklanjutinya sesuai prioritas. Sistem ini juga menyimpan data inspeksi, kondisi instalasi, dan riwayat perawatan secara otomatis, sehingga proses evaluasi dan pengambilan keputusan menjadi lebih akurat dan efisien.


## OOP
Object Oriented Programming (OOP) merupakan fondasi dalam pengembangan aplikasi karena memungkinkan proses pemrograman dilakukan dengan cara yang lebih terstruktur, terorganisir, dan mudah dikembangkan.


### Encapsulation

<img width="662" height="410" alt="image" src="https://github.com/user-attachments/assets/eddd1e02-4850-42b6-b1d3-38c7b0078874" />


Penggunakan Encapsulation pada program agar data penting seperti atribut idUser, username, password, dll tidak bisa diubah sembarangan dari luar kelas. Data hanya bisa diakses lewat method setter/getter, dengan tujuan mencegah perubahan data langsung dari luar class (melindungi integritas data).


### Abstraction

<img width="664" height="176" alt="image" src="https://github.com/user-attachments/assets/e3984697-96c6-4269-abde-d7d3c37335a8" />

Penggunaan abstraction yaitu untuk menyembunyikan detail teknis, hanya menampilkan fungsi yang penting agar sistem lebih mudah dipahami, dan program lain cukup memanggil DatabaseConfig.getConnection() untuk dapat koneksi.


### Inheritance

Class Admin dan Masyarakat menggunakan keyword extends UserBase, agar dapat menggunakan semua properti dan method dari UserBase tanpa menuliskannya ulang.

<img width="959" height="556" alt="image" src="https://github.com/user-attachments/assets/a296b262-ac2a-4e14-a3a0-8683a60722f2" />


### Polymorphism

Class menggunakan polymorphism untuk mewarisi (inheritance) dari class induk, Jadi ini adalah bentuk polymorphism. Satu method dengan nama sama (validateLogin) tapi hasilnya berbeda tergantung role (admin/petugas/masyarakat).
 
<img width="980" height="335" alt="image" src="https://github.com/user-attachments/assets/42b8f500-f0a2-40f7-b9c6-3610cb064b51" />


### Interface 

<img width="1117" height="308" alt="image" src="https://github.com/user-attachments/assets/61e8ea46-d232-4c4d-8399-5d384cfed216" />

Digunakan pada class MasyarakatModel melalui deklarasi implements DatabaseOperation<MasyarakatModel> yang berfungsi sebagai kontrak yang menentukan setiap class yang mengimplementasikannya harus memiliki method insert(), update(), softDelete(), dan getAll().

## Packages
Packages berfungsi mengelompokkan class dan file-file program lainnya ke dalam satu wadah atau folder tertentu. Dengan adanya package, struktur program menjadi lebih teratur, mudah dikelola, serta menghindari konflik nama class yang sama.

<img width="426" height="245" alt="image" src="https://github.com/user-attachments/assets/d5c61a63-8618-45e4-b83b-3e93f7dd8feb" />

### Icon
Package icon diguanakn untuk menyimpan file-file ikon atau gambar, dengan adanya package icon, file tidak akan bercampur dengan class java, sehingga struktur project lebih rapi dan terorganisir.

<img width="386" height="546" alt="image" src="https://github.com/user-attachments/assets/11b02382-56b6-4ac6-99e8-1d69a958f1f5" />


### Koneksi
Package koneksi berfungsi untuk tempat mengelola semua file yang berkaitan dengan koneksi ke database. Terdapat dua file yaitu DatabaseConfig.java yang berfungsi untuk menghubungkan aplikasi ke database seperti MySQL. Kemudian ada file TesKoneksi.java yang berfungsi untuk memastikan bahwa database dapat di akses sebelum aplikasi di gunakan.

<img width="240" height="275" alt="image" src="https://github.com/user-attachments/assets/b02539b8-2b06-4284-85bb-65c001c7b4f8" />


### Main
Package Main berfungsi sebagai pusat logika, yaitu tempat menyimpan semua class yang terkait dengan proses uatama atau tampilan program.

<img width="229" height="362" alt="image" src="https://github.com/user-attachments/assets/af1eddf8-e6e5-4180-a6a4-7a361b36c31c" />


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

### Flowchart

<img width="4645" height="2872" alt="Keseluruhan drawio" src="https://github.com/user-attachments/assets/64582bed-fe5e-422e-978a-70c434e2dd17" />


### Login
<img width="687" height="1197" alt="Login drawio" src="https://github.com/user-attachments/assets/2ece9671-e149-46f7-b633-dcf7bbb0a996" />


### Registrasi
<img width="252" height="1503" alt="Regis drawio" src="https://github.com/user-attachments/assets/dd30bafe-112e-4c76-b07d-43172b8a14df" />


### Petugas
<img width="888" height="1045" alt="Petugas drawio" src="https://github.com/user-attachments/assets/5eac6815-54cc-4865-8c56-3c96a1125824" />


### Masyarakat
<img width="990" height="1242" alt="Masyarakat drawio" src="https://github.com/user-attachments/assets/bff1554d-7a48-49b1-9142-fe8e77d88f2a" />


### Admin
<img width="1030" height="1838" alt="Admin drawio" src="https://github.com/user-attachments/assets/760e7434-0400-49cc-9364-262327a8dac9" />


### Use Case

<img width="787" height="670" alt="use case drawio (1)" src="https://github.com/user-attachments/assets/bf7479e7-86e0-4dcc-9c83-4f7ae922aed6" />


## graphical User Interface (GUI)

### Halaman Landing Page


### Halaman Login 


## Admin

### Halaman Wellcome 

### Halaman Lihat Laporan


### Halaman Hapus laporan


### halaman Registrasi Petugas


### Hamana Ubah Status


### Halaman Edit data Petugas


## Petugas

### Halaman Wellcome 


### Halaman Lihat Laporan


### Halaman Ubah Status


### halaman Tindak lanjut



## Masyarakat

### Halaman Registrasi Masyarakat


### Halaman Wellcome 


### Halaman Buat Laporan


### halaman Lihat Laporan




