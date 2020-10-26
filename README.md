# LatihanVCS
TUGAS PERTEMUAN 4

BAHASA PEMROGRAMAN

TEHNIK INFORMATIKA

UNIVERSITAS PELITA BANGSA

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

![01_download git](../Picture/01_istalasi%20git/01_download%20git.jpg)

![02_istall git](../Picture/01_istalasi%20git/02_istall%20git.jpg)

![03_git bash](../Picture/01_istalasi%20git/03_git%20bash.jpg)

• Selamat, Git sudah terinstal di Windows. Untuk mencobanya,
silahkan buka CMD atau PowerShell, kemudian ketik perintah

``git --version``

![04_git version](../Picture/01_istalasi%20git/04_git%20version.jpg)

**Menambahkan Global Config**

• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
user.name dan user.email

• konfigurasi ini bisa dilakukan untuk global repostiry atau individual
repository.

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi
kegagalan saat menjalankan perintah git commit

• Config Global Repository

``$ git config --global user. name “nama_user”``

``$ git config --global user. email “nama_user”``

![05_git configuration](../Picture/01_istalasi%20git/05_git%20configuration.jpg)

**Membuat Reposiory Local**

• Buka direktory aktif, misal: e:\labs_pemrograman1 (buka
menggunakan Windows Explorer)

• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
sehingga muncul git bash commad

• Buat direktory project praktikum pertama dengan nama Latihan-VCS

``$ mkdir Latihan-VCS``

``$ cd Latihan-VCS``

![01_Membuat Repository Local](../Picture/02_Membuat%20Reposiory%20Local/01_Membuat%20Repository%20Local.jpg)

• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya
masuk kedalam direktori tersebut dengan perintah cd (change
directory)

• direktory aktif menjadi: e:\labs_pemrograman1\Latihan-VCS


**Membuat Reposiory Local**

• Jalankan perintah git init, untuk membuat repository local.

``$ git init``

![02_git init](../Picture/02_Membuat%20Reposiory%20Local/02_git%20init.jpg)

• Repository baru berhasil di inisialisasi, dengan terbentuknya satu
Direktori hidden dengan nama .git

![03_git folder](../Picture/02_Membuat%20Reposiory%20Local/03_git%20folder.jpg)

• Pada direktori tersebut, semua perubahan pada working directory
akan disimpan.

**Menambahkan File baru pada repository**

• Untuk membuat file dapat menggunakan text editor, lalu menyimpan
filenya pada direktori aktif (repository)

• disini kita akan coba buat satu file bernama README.md (text file)

``$ echo “# Latihan-VCS” >> README. md``

![04_Readmi.md](../Picture/02_Membuat%20Reposiory%20Local/04_Readmi.md.jpg)

• File README.md berhasil dibuat.

![05_Readmi.md file](../Picture/02_Membuat%20Reposiory%20Local/05_Readmi.md%20file.jpg)

Menambahkan File baru pada repository
• Untuk menambahkan file yang baru saja dibuat tersebut gunakan
perintah git add.

``$ git add README. md``

• File README.md berhasil ditambahkan

![06_Readmi.md add](../Picture/02_Membuat%20Reposiory%20Local/06_Readmi.md%20add.jpg)

**Commit (Menyimpan perubahan ke database)**

• Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m “komentar commit”

``$ git commit -m “Bahasa Pemrograman Repository Local LatihanVCS”``

![07_git commit](../Picture/02_Membuat%20Reposiory%20Local/07_git%20commit.jpg)

• Perubahan berhasil disimpan.

![08_git commit perubahan tersimpan](../Picture/02_Membuat%20Reposiory%20Local/08_git%20commit%20perubahan%20tersimpan.jpg)

**Membuat repository server**

• Server reopsitory yang akan kita gunakan adalah http://github.com

• Anda harus membuat akun terlebih dahulu.

• Pada laman github, klik tombol start a project, atau

• Dari menu (icon +) klik New Repository

![01_New repository](../Picture/03_github_update%20server/01_New%20repository.jpg)

**Membuat repository server**

• Isi nama repositorynya, misal: LatihanVCS.

![02_Nama repository](../Picture/03_github_update%20server/02_Nama%20repository.jpg)

• lalu klik tombol Create repository

![03_repository](../Picture/03_github_update%20server/03_repository.jpg)

**Menambahkan Remote Repository**

• Remote Repository merupakan repository server yang akan

digunakan untuk menyimpan setiap perubahan pada local repository,
sehingga dapat diakses oleh banyak user.

Alamat url kita

![04_remote server url](../Picture/03_github_update%20server/04_remote%20server%20url.jpg)

• Untuk menambahkan remote repository server, gunakan perintah

git remote add origin [url]

``$ git remote add origin https://github.com/Gunawan1603/LatihanVCS.git``

![05_git remote url](../Picture/03_github_update%20server/05_git%20remote%20url.jpg)

**Push (Mengirim perubahan ke server)**

• Untuk mengirim perubahan pada local repository ke server gunakan
perintah git push.

``$ git push -u origin master``

• Perintah ini akan meminta memasukkan username dan password
pada akun github.com

![06_git push master,masuk paswor hit hub](../Picture/03_github_update%20server/06_git%20push%20master,masuk%20paswor%20hit%20hub.jpg)
![07_after push git push master](../Picture/03_github_update%20server/07_after%20push%20git%20push%20master.jpg)

**Melihat hasilnya pada server repository**

• Buka laman github.com,
arahkan pada repositorinya.

• Maka perubahan akan
terlihat pada laman
tersebut.

![08_hasil di server github](../Picture/03_github_update%20server/08_hasil%20di%20server%20github.jpg)

**Clone Repository**

• Clone repository, pada dasarnya adalah meng-copy repository server
dan secara otomatis membuat satu direktory sesuai dengan nama
repositorynya (working directory).

• Untuk melakukan cloning, gunakan perintah git clone [url]

``$ git clone https://github.com/Gunawan1603/LatihanVCS.git``

![09_git clone Repository](../Picture/03_github_update%20server/09_git%20clone%20Repository.jpg)

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

![10_Markdown Edit](../Picture/03_github_update%20server/10_Markdown%20Edit.jpg)



TERIMA KASIH😊
