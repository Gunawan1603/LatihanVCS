# Latihan-VCS
                                                                                    **TUGAS PERTEMUAN 4
                                                                                  BAHASA PEMROGRAMAN
                                                                                    TEKNIK INFORMATIKA
                                                                               UNIVERSITAS PELITA BANGSA**
NAMA : GUNAWAN
NIM     : 312010191
KELAS : TI.20.B1
DOSEN : Agung Nugroho,S.Kom.,M.Kom
Tugas : Membuat satu repository LatihanVCS dan Buat file README.md

**Instalasi Git**
• Download Git, buka website resminya Git (git-scm.com).
• Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau
menggunakan 64bit, unduh yang 64bit. Begitu juga kalau
menggunakan 32bit.
![01_download git](https://user-images.githubusercontent.com/72991184/96354799-eab1e300-1104-11eb-8c75-856207d00105.jpg)
![02_istall git](https://user-images.githubusercontent.com/72991184/96354802-f3a2b480-1104-11eb-87f3-490ecb9625e2.jpg)
![03_git bash](https://user-images.githubusercontent.com/72991184/96354831-3cf30400-1105-11eb-8e1c-aa5edd6b9e54.jpg)
• Selamat, Git sudah terinstal di Windows. Untuk mencobanya,
silahkan buka CMD atau PowerShell, kemudian ketik perintah
git --version
![04_git version](https://user-images.githubusercontent.com/72991184/96354832-3ebcc780-1105-11eb-98f5-f02726db30f6.jpg)

**Menambahkan Global Config**
• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
user.name dan user.email
• konfigurasi ini bisa dilakukan untuk global repostiry atau individual
repository.
• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi
kegagalan saat menjalankan perintah git commit
• Config Global Repository
$ git config --global user. name “nama_user”
$ git config --global user. email “nama_user”
![05_git configuration](https://user-images.githubusercontent.com/72991184/96354838-6449d100-1105-11eb-94ea-31db31485c7b.jpg)

**Membuat Reposiory Local**
• Buka direktory aktif, misal: e:\labs_pemrograman1 (buka
menggunakan Windows Explorer)
• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
sehingga muncul git bash commad
• Buat direktory project praktikum pertama dengan nama Latihan-VCS
$ mkdir Latihan-VCS
$ cd Latihan-VCS
![01_Membuat Repository Local](https://user-images.githubusercontent.com/72991184/96354873-ae32b700-1105-11eb-945b-b2b8a4ba1ad6.jpg)
• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya
masuk kedalam direktori tersebut dengan perintah cd (change
directory)
• direktory aktif menjadi: e:\labs_pemrograman1\Latihan-VCS

**Membuat Reposiory Local**
• Jalankan perintah git init, untuk membuat repository local.
$ git init
![02_git init](https://user-images.githubusercontent.com/72991184/96354897-f2be5280-1105-11eb-90f6-b457276a942c.jpg)
• Repository baru berhasil di inisialisasi, dengan terbentuknya satu
Direktori hidden dengan nama .git
![03_git folder](https://user-images.githubusercontent.com/72991184/96354909-1e413d00-1106-11eb-8161-e94691595b52.jpg)
• Pada direktori tersebut, semua perubahan pada working directory
akan disimpan.

**Menambahkan File baru pada repository**
• Untuk membuat file dapat menggunakan text editor, lalu menyimpan
filenya pada direktori aktif (repository)
• disini kita akan coba buat satu file bernama README.md (text file)
$ echo “# Latihan-VCS” >> README. md
![04_Readmi md](https://user-images.githubusercontent.com/72991184/96354932-652f3280-1106-11eb-997a-daf0c6fb3dbc.jpg)
• File README.md berhasil dibuat.
![05_Readmi md file](https://user-images.githubusercontent.com/72991184/96354944-7ed07a00-1106-11eb-98b9-0b342bd64039.jpg)

Menambahkan File baru pada repository
• Untuk menambahkan file yang baru saja dibuat tersebut gunakan
perintah git add.
$ git add README. md
• File README.md berhasil ditambahkan
![06_Readmi md add](https://user-images.githubusercontent.com/72991184/96354964-b4756300-1106-11eb-9e2b-df14cab28a45.jpg)

**Commit (Menyimpan perubahan ke database)**
• Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m “komentar commit”
$ git commit -m “Bahasa Pemrograman Repository Local LatihanVCS”
![07_git commit](https://user-images.githubusercontent.com/72991184/96354995-38c7e600-1107-11eb-95ae-f3c212b48270.jpg)
• Perubahan berhasil disimpan.
![08_git commit perubahan tersimpan](https://user-images.githubusercontent.com/72991184/96354996-38c7e600-1107-11eb-97e9-2570e96e78ba.jpg)

**Membuat repository server**
• Server reopsitory yang akan kita gunakan adalah http://github.com
• Anda harus membuat akun terlebih dahulu.
• Pada laman github, klik tombol start a project, atau
• Dari menu (icon +) klik New Repository
![01_New repository](https://user-images.githubusercontent.com/72991184/96355033-96f4c900-1107-11eb-9569-708d5ec9e6a5.jpg)

**Membuat repository server**
• Isi nama repositorynya, misal: LatihanVCS.
![02_Nama repository](https://user-images.githubusercontent.com/72991184/96355042-a2e08b00-1107-11eb-989b-57eeb3c113f5.jpg)
• lalu klik tombol Create repository
![03_repository](https://user-images.githubusercontent.com/72991184/96355092-15ea0180-1108-11eb-8c7a-901951a7b4b8.jpg)

**Menambahkan Remote Repository**
• Remote Repository merupakan repository server yang akan
digunakan untuk menyimpan setiap perubahan pada local repository,
sehingga dapat diakses oleh banyak user.
Alamat url kita
![04_remote server url](https://user-images.githubusercontent.com/72991184/96355146-9b6db180-1108-11eb-82cb-c52babe8842e.jpg)

• Untuk menambahkan remote repository server, gunakan perintah
git remote add origin [url]
$ git remote add origin https://github.com/Gunawan1603/LatihanVCS.git
![05_git remote url](https://user-images.githubusercontent.com/72991184/96355114-56497f80-1108-11eb-9469-0369d40bfd80.jpg)

**Push (Mengirim perubahan ke server)**
• Untuk mengirim perubahan pada local repository ke server gunakan
perintah git push.
$ git push -u origin master
• Perintah ini akan meminta memasukkan username dan password
pada akun github.com
![06_git push master,masuk paswor hit hub](https://user-images.githubusercontent.com/72991184/96355158-bfc98e00-1108-11eb-93ff-a4e6f5acc5a7.jpg)
![07_after push git push master](https://user-images.githubusercontent.com/72991184/96355185-01f2cf80-1109-11eb-9cb2-e62bf079cc69.jpg)

**Melihat hasilnya pada server repository**
• Buka laman github.com,
arahkan pada repositorinya.
• Maka perubahan akan
terlihat pada laman
tersebut.
![08_hasil di server github](https://user-images.githubusercontent.com/72991184/96355193-1fc03480-1109-11eb-953d-9880ae5b7226.jpg)

**Clone Repository**
• Clone repository, pada dasarnya adalah meng-copy repository server
dan secara otomatis membuat satu direktory sesuai dengan nama
repositorynya (working directory).
• Untuk melakukan cloning, gunakan perintah git clone [url]
$ git clone https://github.com/Gunawan1603/LatihanVCS.git
![09_git clone Repository](https://user-images.githubusercontent.com/72991184/96355211-50a06980-1109-11eb-90a3-88452a678c76.jpg)

**Kegunaan file README.md**
• Apabila kita menggunakan github, untuk memberikan penjelasan
awal pada project yang kita buat, maka dapat menggunakan sebuah
file yang bernama README.md
• Pada file tersebut kita dapat membuat dokumentasi awal dari setiap
project yang kita buat untuk memberikan penjelasan atau sekedar
cara penggunaan dari aplikasi yang kita kembangkan.
• Penulisan file README.md berbasis teks, dan untuk pemformatannya
menggunakan Markdown format.
• untuk lebih jelasnya, dapat anda pelajari cara penggunaan markdown
pada url berikut: https://guides.github.com/features/masteringmarkdown/

                                                                               **TERIMAKASIH**
