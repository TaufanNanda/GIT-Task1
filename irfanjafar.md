# GIT

Git adalah salah satu tool yang sering digunakan dalam proyek pengembangan software.

Git bahkan menjadi tool yang wajib dipahami oleh programmer, karena banyak digunakan di mana-mana.

Pada kesempatan ini kita akan belajar Git dari dasar.

Artikel ini hanya akan membahas pengenalan Git saja. Untuk mempelajari Git lebih lanjut, saya sudah menyediakan link di bagian akhir.

Mengenal Git
Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.

Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.

Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.

Git ini sebenernya memudahkan programmer untuk mengetahui perubahan source codenya daripada harus membuat file baru seperti Program.java, ProgramRevisi.java,  ProgramRevisi2.java, ProgramFix.java. Selain itu, dengan git kita tak perlu khawatir code yang kita kerjakan bentrok, karena setiap developer bias membuat branch sebagai workspacenya.Fitur yang tak kalah keren lagi, pada git kita bisa memberi komentar pada source code yang telah ditambah/diubah, hal ini mempermudah developer lain untuk tahu  kendala apa yang dialami developer lain.

Untuk mengetahui bagaimana menggunakan git, berikut perintah-perintah dasar git:

Git init : untuk membuat repository pada file lokal yang nantinya ada folder .git
Git status : untuk mengetahui status dari repository lokal
Git add : menambahkan file baru pada repository yang dipilih
Git commit : untuk menyimpan perubahan yang dilakukan, tetapi tidak ada perubahan pada remote repository.
Git push : untuk mengirimkan perubahan file setelah di commit ke remote repository.
Git branch : melihat seluruh branch yang ada pada repository
Git checkout : menukar branch yang aktif dengan branchyang dipilih
GIt merge : untuk menggabungkan branch yang aktif dan branch yang dipilih
Git clone : membuat Salinan repository lokal

fitur fitur yang ada didalam GIT berikut adalah:

Version control system yang terdistribusi, GIT menggunakan pendekatan peer to peer, tidak seperti yang lainnya seperti Subversion (SVN) yang menggunakan model client-server.
GIT memungkinkan developer untuk memiliki branch kode yang independent dan massive. Membuat, menghapus dan menggabungkan branch tersebut menjadi lebih cepat, lancar dan tidak butuh waktu yang lama.
GIT bersifat atomic, adalah sebuah tindakan akan benar-benar diselesaikan dengan lengkap atau sama sekali gagal. Ini sangat penting, karena di beberapa version control system seperti CVS, operasinya bersifat non-atomic. Jika ada operasi yang ‘gantung’ dan terkait dengan repository, kondisi repository menjadi tidak stabil.
Media penyimpanan GIT yaitu dalam folder .git. Berbeda dengan VCS lain seperti SVN atau CVS, dimana metadata file disimpan dalam folder tersembunyi seperti .cvs, .svn, .etc.
GIT memiliki data model yang dapat membantu memastikan integritas cryptographic yang ada dalam repository. Sehingga setiap kali sebuah file ditambahkan atau di-commit, checksum-nya akan diciptakan; sama hal nya, juga di-retrieve lewat checksum-nya juga.
GIT memiliki staging area atau index. Dengan stagin area, developer bisa memformat commit dan membuatnya bisa di-review sebelum benar-benar diterapkan.
GIT sangat sederhana dalam penggunannya. Untuk memulai, Anda bisa membuat repository atau men-checkout yang sudah ada. Setelah instalasi, perintah git-init akan men-setup semuanya.Semua orang yang terlibat dalam pengkodean proyek akan menyimpan database Git, sehingga akan memudahkan dalam mengelola proyek baik online maupun offline.

Dalam Git terdapat merge untuk menyebut aktifitas penggabungan kode.

Sedangkan pada VCS (Version Control System) yang terpusat… database disimpan dalam satu tempat dan setiap perubahan disimpan ke sana..