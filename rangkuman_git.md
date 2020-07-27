### GIT

**Git** adalah salah satu sistem pengontrol versi (*Version Control System*/VCS) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.

Git bukan satu-satunya VCS yang ada, berikut adalah beberapa VCS yang juga populer digunakan:  

**Centralized VCS**                             **Distributed VCS**
* Subversion (svn)                              * Git (git)  
* CVS (cvs)                                     * Mercurial (hg)  
* Perforce                                      * Bazaar (bzr)

**Centralized VCS**
Sistem kerja dari Centralized Version Control seperti hubungan client-server, dimana sebuah repositori diletakkan pada server dan memberikan akses kepada semua client.  
Ketika terjadi perubahan pada repositori, programmer dapat melakukan update selama masih terhubung ke server. Karena bergantung pada server, maka apabila server dalam keadaan mati tentunya maka programmer tidak dapat menyimpan perubahan terhadap code yang telah dimodifikasi.  

**Distributed VCS**
Pada Distributed VCS, programmer memiliki seluruh salinan repository baik file maupun history-nya. Kelebihannya adalah kita dapat melakukan semua operasi secara lokal kecuali pada saat melakukan sharing repositori.

**Kenapa Programmer Perlu Menggunakan VCS?**
VCS dapat meng-track setiap modikasi yang dilakukan pada source code, apabila terjadi kesalahan pada saat modifikasi source code, kita dapat kembali pada versi awal sebelum terjadi kesalahan.

Misalnya kita sedang membangun sebuah aplikasi, tentunya sangat wajar jika kita sebagai seorang programmer melakukan revisi source code berulang kali. Revisi code bisa dilakukan pada satu file atau lebih. Jika seandainya client meminta kita untuk menghilangkan atau membatalkan sebuah fitur pada aplikasi tersebut, padahal sebelumnya si client tersebut yang meminta penambahan fitur. Tentunya akan merepotkan sekali melakukan proses revisi code, apalagi harus dilakukan proses revisi code pada banyak file. Dengan menggunakan VCS, permasalahan tersebut dapat diatasi. Version control mencatat informasi perubahan atas apa-apa saja yang telah dirubah, tanggal serta informasi user yang melakukan perubahan (modifikasi) source code tersebut. Dengan demikian kita dapat kembali pada versi awal sebelum penambahan fitur tersebut.

**Perintah-Perintah Umum Pada Git**
* git **init**  : Menginilisasi repository git baru
* git **clone** : Membuat salinan repository git yang sudah ada
* git **status**: Mengecek status repository git
* git **add**   : Menambahkan file pada folder git untuk di staging
* git **commit -m 'Commit Message'**: Untuk menyimpan perubahan file
* git **log**   : Melihat history hasil commit
* git **pull**  : Mendapatkan perubahan file pada repository yang di remote
* git **push**  : Untuk *push* perubahan ke repository yang di remote
* git **diff**  : Melihat perbedaan file yang sebelum dan sesudah diubah
* git **merge** : Untuk menyatukan branch
* git **branch**: Untuk menggunkana branch yang diinginkan
dan masih banyak lagi perintah pada Git lainnya