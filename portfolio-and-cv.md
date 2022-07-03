Assignment git and github
Jessica Nurzabrina (team 19)
Kamu adalah seorang programer yang ingin mendaftar kesalah satu perusahaan terkenal, oleh karena itu kamu sudah memulai untuk mempersiapkan CV dan Portfolio. Namun kamu tidak ingin membuat banyak CV dan Portfolio dengan model seperti ini

cv.pdf
cv-final.pdf
cv-final-v2.pdf
Oleh karenanya kamu berinisiatif untuk menggunakan Git, lalu langkah yang kamu lakukan adalah:

1. membuat sebuah folder kosong dengan namamu sendiri
    (mkdir jessica-nurzabrina)
2. membuat sebuah file di dalam folder tersebut dengan nama README.md,  isi file tersebut dengan kalimat
"Halo perkenalkan aku halaman utama"
    (echo "Halo perkenalkan aku halaman utama" >> README.md)
3. inisialisasi folder tersebut dengan Git, kemudian simpan perubahan menggunakan commit dengan pesan
"First commit"
    (git init ; git add README.md ; git commit -m "First Commit")
4. Ganti teks sebelumnya dengan `"Hello world" 
    (nano README.md ; kemudian edit tulisan menjadi "Hello World" ; lalu ctrl+O untuk menyimpan, kemudian tekan ctrl+X)
5. Tampilkan isi teks tersebut pada command line menggunakan command cat (git cat-file README.md)
6. Ternyata kamu tidak ingin perubahan tersebut, dan ingin kembali ke perubahan seperti commit yang terakhir. Lakukan teknik git backtracking untuk mengembalikan ke perubahan commit yang terakhir. (git reset)
7. buat branch baru dengan nama cv, hal ini berguna agar histori kita tidak tercampur (git checkout -b CV)
8. pindah branch ke dalam cv, kemudian buat file dengan nama cv.txt dan isi file tersebut dengan kalimat:
"Ini adalah file CV"
    (echo "Ini adalah file CV" >> cv.txt)
9. kemudian simpan perubahan menggunakan commit dengan pesan
"Initial CV"
    (git add cv.txt ; git commit -m "Initial CV")
10. tambahkan 3 perusahaan yang akan kamu lamar, dan setiap menuliskan 1 nama perusahaan kamu harus melakukan dokumentasi dan menyimpan perubahan menggunakan commit
    (nano cv.txt ; kemudian tambahkan nama perusahaan ; lalu ctrl+O untuk menyimpan, kemudian tekan ctrl+X ; git add . ; git commit -m "menambahkan perusahaan 1"
    nano cv.txt ; kemudian tambahkan nama perusahaan ; lalu ctrl+O untuk menyimpan, kemudian tekan ctrl+X ; git add . ; git commit -m "menambahkan perusahaan 2"
    nano cv.txt ; kemudian tambahkan nama perusahaan ; lalu ctrl+O untuk menyimpan, kemudian tekan ctrl+X ; git add . ; git commit -m "menambahkan perusahaan 3")
11. kembali ke branch master
    (git checkout master)
12. ubah file README.md menjadi
Halo perkenalkan aku halaman utama

Ini adalah update pertama pada branch master
jangan lupa untuk menyimpan perubahan menggunakan commit dengan pesan
"update master pertama"
    (nano README.md ; kemudian edit tulisan menjadi 
    "Halo perkenalkan aku halaman utama 
    Ini adalah update pertama pada branch master" ; lalu ctrl+O untuk menyimpan, kemudian tekan ctrl+X ; git add . ; git commit -m "update master pertama")
13. gabungkan branch cv ke dalam branch master menggunakan perintah git merge (git checkout main ; git merge CV)
14. unggah Git Repository project tersebut tersebut ke dalam GitHub
    (git push origin)