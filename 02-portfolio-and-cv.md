1. membuat sebuah folder kosong dengan **namamu sendiri**. **mkdir Ariel**
2. membuat sebuah file di dalam folder tersebut dengan nama `README.md`, isi file tersebut dengan kalimat<br>`"Halo perkenalkan aku halaman utama"`. **echo "Halo perkenalkan aku halaman utama" > README.md**
3. **inisialisasi** folder tersebut dengan Git, kemudian simpan perubahan menggunakan `commit` dengan pesan<br>`"First commit"`. 
<br>**git init .<br>git add .<br>git commit -m "First commit"**
4. Ganti teks sebelumnya dengan `"Hello world"`. **echo "Hello world" > README.md**
5. Tampilkan isi teks tersebut pada command line menggunakan command `cat`. **cat README.md**
6. Ternyata kamu tidak ingin perubahan tersebut, dan ingin kembali ke perubahan seperti commit yang terakhir. Lakukan teknik git backtracking untuk mengembalikan ke perubahan commit yang terakhir. **git checkout README.md**
7. buat `branch` baru dengan nama `cv`, hal ini berguna agar histori kita tidak tercampur. **git branch cv**
8. pindah `branch` ke dalam `cv`, kemudian buat file dengan nama `cv.txt` dan isi file tersebut dengan kalimat:<br>`"Ini adalah file CV"`. <br>**git checkout cv<br>echo "Ini adalah file CV" > cv.txt**
9. kemudian simpan perubahan menggunakan `commit` dengan pesan<br>`"Initial CV"`. <br>**git add .<br>git commit -m "Initial CV"**
10. tambahkan **3 perusahaan** yang akan kamu lamar, dan setiap menuliskan 1 nama perusahaan kamu harus melakukan dokumentasi dan menyimpan perubahan menggunakan `commit`. <br>**echo "perusahaan pertama" >> cv.txt<br>git commit -m "menambahkan perusahaan pertama"<br>echo "perusahaan kedua" >> cv.txt<br>git commit -m "menambahkan perusahaan kedua"<br>echo "perusahaan ketiga" >> cv.txt<br>git commit -m "menambahkan perusahaan ketiga"**
11. kembali ke `branch master`. **git checkout master**
12. ubah file `README.md` menjadi
    ```
    Halo perkenalkan aku halaman utama

    Ini adalah update pertama pada branch master
    ```
    jangan lupa untuk menyimpan perubahan menggunakan `commit` dengan pesan<br>`"update master pertama"`. <br>**echo "Halo perkenalkan aku halaman utama \n\nIni adalah update pertama pada branch master" > README.md<br>git commit -m "update master pertama"**
13. gabungkan branch `cv` ke dalam branch `master` menggunakan perintah `git merge`. **git merge cv**
14. unggah Git Repository project tersebut tersebut ke dalam GitHub. <br>**Buat repositori baru di github, lalu copy link repositorinya<br>Kemudian, buka terminal<br>Ketik git remote add origin url_repositori<br>Setelah itu, ketik git push -u origin master**
