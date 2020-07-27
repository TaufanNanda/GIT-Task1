Rangkuman GIT
=============

1.Pengertian
------------

**Git** adalah _version control system_ yang digunakan para developer untuk mengembangkan software secara bersama-bersama. Fungsi utama git yaitu mengatur versi dari _source code_ program anda dengan memberi tanda baris dan kode mana yang ditambah atau diganti.

**Git** ini sebenarnya memudahkan programmer untuk mengetahui perubahan _source code_-nya daripada harus membuat file baru seperti Program.java, ProgramRevisi.java,  ProgramRevisi2.java, ProgramFix.java. Selain itu, dengan git kita tak perlu khawatir code yang kita kerjakan bentrok, karena setiap developer bias membuat branch sebagai workspacenya.Fitur yang tak kalah keren lagi, pada git kita bisa memberi komentar pada source code yang telah ditambah/diubah, hal ini mempermudah developer lain untuk tahu  kendala apa yang dialami developer lain.

Untuk mengetahui bagaimana menggunakan git, berikut perintah-perintah dasar git:

* Git init : untuk membuat repository pada file lokal yang nantinya ada folder .git
* Git status : untuk mengetahui status dari repository lokal
* Git add : menambahkan file baru pada repository yang dipilih
* Git commit : untuk menyimpan perubahan yang dilakukan, tetapi tidak ada perubahan pada remote repository.
* Git push : untuk mengirimkan perubahan file setelah di commit ke remote repository.
* Git branch : melihat seluruh branch yang ada pada repository
* Git checkout : menukar branch yang aktif dengan branchyang dipilih
* GIt merge : untuk menggabungkan branch yang aktif dan branch yang dipilih
* Git clone : membuat Salinan repository lokal

Contoh dari software _version control system_ adalah github, bitbucket, snowy evening, dan masih banyak lagi. Jika anda sebagai developer belum mengetahui fitur git ini, maka anda wajib mencoba dan memakainya. Karena banyak manfaat yang akan didapat dengan git ini.

2.Cara Install
--------------

* Windows
  Menginstall GIT di Windows sangat mudah, cukup dengan mendownload dan menjalankan instalasinya. Ikuti langkah berikut ini untuk meng-install GIT di Windows:
  1. Download installer GIT untuk Windows.
  2. Setelah download, buka file tersebut untuk menjalankan proses instalasi. Ikuti semua instruksi, klik Next dan Finish hingga semua proses instalasi selesai.
  3. Jalankan perintah berikut ini di terminal:
     `git config --global user.name "Username Anda"`
     `git config --global user.email "example@email.com"`

* MacOS
  Ada banyak cara meng-install GIT di perangkat Mac. Bisa jadi GIT sudah terinstall di komputer Anda jika Anda telah memiliki aplikasi XCode sebelumnya. Jalankan perintah berikut ini di terminal untuk memastikan:
  `git --version`
  Jika Anda mendapatkan output seperti `git version 2.7.0 (Apple Git-66)`, Anda beruntung. Namun jika tidak, ikuti langkah berikut ini:
  1. Download installer terbaru untuk Mac.
  2. Ikuti instruksi di layar dan selesaikan proses instalasi.
  3. Sekali lagi, ketikkan perintah `git --version` untuk memastikan bahwa instalasi telah berhasil.
  4. Jalankan perintah berikut ini di terminal Anda untuk mengkonfigurasi email Anda dan username yang digunakan untuk akun GIT:
     `git config --global user.name "Username Anda"`
     `git config --global user.email "example@email.com"`

* Linux
  Jika Anda adalah pengguna Linux, mungkin Anda telah terbiasa meng-install software dan paket di komputer Anda menggunakan perintah apt-get atau yum install. Begitu juga dengan instalasi GIT:

  **Untuk pengguna Debian/Ubuntu (apt-get):**
    1. Buka terminal dan jalankan perintah berikut ini:
       `Sudo apt-get update`
	   `Sudo apt-get install git`
	2. Cek apakah instalasi sudah berhasil dengan menggunakan `git --version`
	3. Jalankan perintah berikut di terminal untuk mengkonfigurasikan email Anda dan username yang digunakan dengan akun GIT Anda:
       `git config --global user.name "Username Anda"`
       `git config --global user.email "example@email.com"`

  **Fedora (yum/dnf):**
    Anda bisa mengekstrak paket GIT menggunakan yum atau dnf.
	1. Buka terminal dan jalan perintah ini:
	   `Sudo dnf install git`
	   `Sudo yum install git`
    2. Cek instalasi dengan menggunakan `git --version`
	3. Jalankan perintah berikut di terminal untuk mengkonfigurasikan email Anda dan username yang digunakan dengan akun GIT Anda:
       `git config --global user.name "Username Anda"`
       `git config --global user.email "example@email.com"`

3.Penggunaan
------------

Sekarang, setelah GIT di-install di komputer Anda, mari kita pelajari dasar GIT dan bagaimana cara menggunakan GIT.

* **Membuat/mengatur/mengambil repository:** Repository adalah asset yang paling kuat dari semua project versioning. Untuk mengubah direktori menjadi repository GIT, jalankan perintah `git init <directory>`. Folder bernama .gt akan muncul di direktori bila perintah tersebut telah dijalankan. Kemudian, jika Anda telah memiliki direktori sebelumnya dan ingin mengambilnya, Anda bisa menggunakan perintah git clone. Jika Anda ingin mencoba mengambil repository lokal, gunakan perintah ini:
`git clone /path/to/local/repository`
Jika Anda ingin memeriksa repository yang tersimpan, gunakan:
`git clone user.name@host:/path/to/remote/repository`
Jika Anda memiliki akun di Hostinger, Anda bisa dengan mudah menyalin dan mengatur repository melalui **Member Area -> GIT**.

* **Alur kerja:** Setelah repository selesai dibuat, kita akan membahas tentang struktur pada GIT. Setiap repository lokal memiliki 3 cabang, yaitu: direktori kerja yang mengandung file; index berperan sebagai staging area dan HEAD yang menjadi penunjuk commit terakhir yang dilakukan oleh user. Jadi, seperti inilah cara kerjanya: user menambahkan file atau melakukan perubahan dari direktori kerja ke index (staging area) dan setelah di-review, file atau perubahan di-commit ke HEAD.

* **Perintah ADD dan COMMIT:** Perubahan yang diajukan atau file tambahan akan ditambahkan ke index dengan menggunakan perintah add. Untuk menambahkan file, perintah sederhananya adalah:
`git add <file_name>`
Jika Anda cukup yakin untuk melakukan perubahan langsung di HEAD, Anda langsung gunakan perintah commit. Contohnya:
`git commit –m “Tambahkan catatan untuk commit Anda”`

* **Mengirim perubahan:** Setelah Anda melakukan commit perubahan (dan sudah yakin siap dikirim ke repository asli), Anda bisa menggunakan perintah push.Setelah `git push origin master` dijalankan dari direktori kerja, perubahan yang ada di HEAD akan dikirim ke remote repository. Seperti yang telah disebutkan sebelumnya, master bisa diganti  menjadi nama branch dimana perubahan ingin Anda commit.
Jika repository yang ada saat ini belum di-clone dan Anda ingin membuat sambungan antara repository dan remote server, maka jalankanlah perintah ini:
`git remote add origin <server>`
_(Catatan: Ganti `<server>` dengan alamat remote server.)_
Setelah di-clone, perubahan yang telah dibuat akan dikirim ke server.

* **Branches:** Fitur keren lainnya dari GIT adalah kemampuannya untuk memungkinkan developer dan project manager untuk membuat branch independen yang berbeda dalam 1 project. Tujuan utama branch adalah untuk membuat fitur namun tetap mengisolasinya dari yang lain. Branche default di project adalah master branch. Karena banyak branch yang dibutuhkan bisa dibuat dan digabungkan dengan master branch.Branch baru bisa dibuat dengan menggunakan perintah berikut ini:
`git checkout -b nama_branch *`
Jika Anda ingin kembali ke master branch utama, jalankan perintah ini:
`git checkout master`
Untuk membuat branch bisa digunakan oleh pengguna lain, Anda harus mengirimkannya ke remote repository melalui perintah ini:
`git push origin nama_branch`

* **Update & Merging:** Jika Anda ingin meng-update direktori kerja lokal Anda saat ini ke yang paling baru dari remote repository, jalankan perintah git pull.Untuk menggabungkan branch lain ke yang sudah aktif, gunakan:
`git merge nama_branch`
Jika Anda melakukan pull atau merge, GIT akan selalu mencoba menangani conflict  sendiri, namun kadang-kadang juga gagal. Jika terjadi kegagalan karena conflict, maka pengguna harus melakukan resolve conflict secara manual. Setelah Anda meng-edit file (untuk menghapus conflict), tandai sebagai merged dengan perintah:
`git add <nama_file>`
Jika setelah merging Anda ingin melihat perubahan, jalan perintah:
`git diff <nama_sumber_branch> <nama_target_branch>`

* **Tagging:** Sebelum merilis update/perubahan apapun, sangat disarankan untuk membuat tag. Untuk melakukannya di GIT, gunakan perintah:
`git tag nama_tag nomor_commit`

* **Log:** Catatan history dari repository bisa dipelajari dari log. Perintah git log yang menampilkannya. Untuk menampilkan commit yang dibuat oleh seorang pengguna, Anda bisa menggunakan perintah:
`git log --author =Nama`
Log yang terkompresi (1 commit per baris) bisa dilihat dengan:
`git log --pretty=oneline`
Untuk hanya melihat file yang berubah:
`git log --name-status`

* **Mengganti perubahan di lokal:** Jika Anda tidak sengaja membuat kesalahan dan ingin kembali ke perubahan normal yang sebelumnya, gunakan perintah:
`git checkout -- <filename>`
Dengan melakukan hal tersebut, akan mengganti perubahan di direktori kerja dengan yang terakhir ada di HEAD. Perubahan apapun yang ditambahkan ke index tidak akan terkena dampak.
Sebaliknya, jika semua perubahan/commit di-drop dan master branch lokal dibutuhkan untuk menunjukkan history terakhir dari server, jalankan perintah:
`git fetch origin`
`git reset --hard origin/master`