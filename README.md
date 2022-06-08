Nama : Nelviana Dwi Lestari

Kelas : TI.20.D1

NIM : 312010086

Matkul : Pemograman Web

Untuk mengaktifkan ekstentsi tersebut, melalu XAMPP Control Panel, pada bagian Apache klik Config -> PHP.ini

![1](https://user-images.githubusercontent.com/101821904/172718867-e9dc4f46-6b34-4c64-a0e4-f8437840339f.png)
![2](https://user-images.githubusercontent.com/101821904/172718911-c0165c81-f546-431b-87ad-24c8bb234948.png)

Unduh Codeigniter dari website https://codeigniter.com/download Extrak file zip Codeigniter ke direktori htdocs/lab11_ci. Ubah nama direktory framework-4.x.xx menjadi ci4. Buka browser dengan alamat http://localhost/lab11_ci/ci4/public

![3](https://user-images.githubusercontent.com/101821904/172718958-bc0f71f3-0977-47fe-ba3e-1b542d3f508a.png)

Menjalankan CLI (Command Line Interface) Codeigniter 4 menyediakan CLI untuk mempermudah proses development. Untuk mengakses CLI buka terminal/command prompt.
![44](https://user-images.githubusercontent.com/101821904/172719000-ff32a1a1-e7f3-4e41-bb35-1e3010330211.png)

Arahkan lokasi direktori sesuai dengan direktori kerja project dibuat (xampp/htdocs/lab11_ci/ci4/) Perintah yang dapat dijalankan untuk memanggil CLI Codeigniter adalah: php spark
![5](https://user-images.githubusercontent.com/101821904/172719022-b92e2093-285b-4349-a08e-d588ec73fcf4.png)

Semua jenis error akan ditampilkan sama. Untuk memudahkan mengetahui jenis errornya, maka perlu diaktifkan mode debugging dengan mengubah nilai konfigurasi pada environment variable CI_ENVIRINMENT menjadi development.
![6](https://user-images.githubusercontent.com/101821904/172719052-4ec472e9-84f0-4e4f-b978-0301cd28ee6f.png)
![7](https://user-images.githubusercontent.com/101821904/172719072-6a14a1ed-75ed-428c-8945-d1335dd97841.png)

Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode.
![8](https://user-images.githubusercontent.com/101821904/172719109-19ff4a1e-bf32-4970-90ce-6ed3ec825b9c.png)

Struktur Direktori Untuk lebih memahami Framework Codeigniter 4 perlu mengetahui struktur direktori dan file yang ada. Buka pada Windows Explorer atau dari Visual Studio Code -> Open Folder.
![9](https://user-images.githubusercontent.com/101821904/172719154-6f882a54-256e-4a11-ac8d-626ec2483f47.png)

Router terletak pada file app/config/Routes.php
![10](https://user-images.githubusercontent.com/101821904/172719198-28bee015-80d7-4867-886f-6285df8a7134.png)

membuat Route Baru. Tambahkan kode berikut di dalam Routes.php $routes->get('/about', 'Page::about'); $routes->get('/contact', 'Page::contact'); $routes->get('/faqs', 'Page::faqs');
![11](https://user-images.githubusercontent.com/101821904/172719215-409385b9-3f49-4139-8204-a7f69387a634.png)

php spark routes
![12](https://user-images.githubusercontent.com/101821904/172719253-3f35099d-c996-4603-a7ca-6e973ad0093f.png)
![13](https://user-images.githubusercontent.com/101821904/172719275-49df7416-13d9-4c51-b2e5-25d51d76e170.png)

Membuat Controller
![14](https://user-images.githubusercontent.com/101821904/172719301-703de6ea-5571-4366-b2dd-72c78fb399e7.png)

Hasil browser
![15](https://user-images.githubusercontent.com/101821904/172719331-99c2b0a2-9fd2-4099-b8af-f36f91f989a6.png)

Tambahkan method baru pada Controller Page seperti berikut.
![16](https://user-images.githubusercontent.com/101821904/172719360-9d741d54-8d86-496d-b571-e09c4d077ea8.png)

![17](https://user-images.githubusercontent.com/101821904/172719380-059c7643-af48-4fd8-8d0f-746a403609bc.png)

Membuat View Selanjutnya adalam membuat view untuk tampilan web agar lebih menarik. Buat file baru dengan nama about.php pada direktori view (app/view/about.php) kemudian isi kodenya seperti berikut.
![18](https://user-images.githubusercontent.com/101821904/172719414-158da5cb-f6f3-4ca7-a926-ba5244a9bf60.png)

Ubah method about pada class Controller Page menjadi seperti berikut:
![19](https://user-images.githubusercontent.com/101821904/172719441-a03ce2b8-460e-454f-b2a5-40819872c43b.png)

Hasil browser
![20](https://user-images.githubusercontent.com/101821904/172719470-9557222a-a54f-433e-b776-84c8efa7ad7c.png)

Buat file css pada direktori public dengan nama style.css (copy file dari praktikum lab4_layout. Kita akan gunakan layout yang pernah dibuat pada praktikum 4
.![a](https://user-images.githubusercontent.com/101821904/172719497-e1ecb1c5-7ad2-4aa7-a898-a6ce2885bb63.png)

Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php File app/view/template/header.php
![21](https://user-images.githubusercontent.com/101821904/172719608-6383dc98-0b88-4e29-8869-4f97e20bcb63.png)

File app/view/template/footer.php
![22](https://user-images.githubusercontent.com/101821904/172719640-7cc5c398-4f7e-42d8-836a-4c66933ba16f.png)
![23](https://user-images.githubusercontent.com/101821904/172719732-8069e92d-58e7-4f2a-8ef3-88753cd3f6da.png)

ertanyaan dan Tugas Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.

About
![24](https://user-images.githubusercontent.com/101821904/172719791-3726b163-2d47-4de8-8688-05c0e656e5ba.png)

hasil web
![25](https://user-images.githubusercontent.com/101821904/172719806-39b0cfb2-0600-4560-b14f-ac10ded9ffb5.png)
