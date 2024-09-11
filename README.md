# Adzkia_Zulfa_Amara_09011282328039_Sistem-Operasi_Tugas-04

## 1. Lihat peralatan I/O, character device, yang ada pada system komputer. 
## Menggunakan perintah ls /dev/: Ini akan menampilkan daftar semua perangkat di direktori /dev, termasuk character device
<img width="191" alt="langkah 1_Part 1_Tugas 04" src="https://github.com/user-attachments/assets/78529018-d7d0-4ca5-bd9c-2720b67bf4a7">

## Perintah ls -l /dev | grep '^c' digunakan untuk menampilkan daftar character devices di direktori /dev.

<img width="250" alt="langkah 1_Part 2_tugas04" src="https://github.com/user-attachments/assets/09358f6f-b541-4305-9349-ac9875b85b9e">


## 2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5. 

<img width="404" alt="langkah 2_Tugas 04" src="https://github.com/user-attachments/assets/f4d69cba-7da5-45b5-a227-36dad5f89dd8">

### a.Tulis Perintah ls di Linux digunakan untuk menampilkan daftar file dan direktori di dalam sebuah direktori. 
### b. setelah mengetahu direktori yang muncul,beri perintah mkdir di Linux digunakan untuk membuat direktori baru yaitu Latihan5.
### c. lihat kembali ls, lalu pindah ke direktori Latihan5 dengan perintah cd dan buat direktori baru  januari, februari, maret dengan mkdir


## 3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret.

## buat file nano dataku.txt untuk memebuat file,isi dengan Nama, Nim dan Alamat, perintah cat untuk melihat isi data. dan gunkan cp untuk mengcopy dataku ke direktori februari dam maret. 

<img width="434" alt="Langkah 3_Part2_Tugas 04" src="https://github.com/user-attachments/assets/a9981164-f64e-4bda-a30d-03dbf00d2782">

## 4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.
Gunakan perintah chmod untuk menambahkan izin write (w) bagi grup (g) dan orang lain (o).

<img width="371" alt="Langkah 4_Tugas 5 fix" src="https://github.com/user-attachments/assets/396e4d7b-1106-4ecc-a942-b3a284b39001">

Untuk memeriksa apakah perubahan izin telah berhasil, gunakan perintah ls -l untuk melihat izin file

## 5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute. 

<img width="381" alt="Langkah_5_Februari_Perintah" src="https://github.com/user-attachments/assets/4e083fea-62e1-49af-9efd-e8e7c5d984d5">

### a. chmod  u+rwx: Menambahkan izin read, write, dan execute untuk pemilik (user) 
### b. chmod go-w : digunakan untuk menghapus izin write dari group dan others
### c. chmod  go+rx: Menambahkan izin read dan execute untuk group dan others.
### d. ls -l nUntuk memeriksa apakah perubahan izin sudah diterapkan


## 6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute. 

<img width="341" alt="Langkah6_Tugas 04" src="https://github.com/user-attachments/assets/037b82db-60c3-470a-a410-f90bcf002ce7">

sudo chmod ugo+rwx dataku.txt. Perintah sudo chmod ugo+rwx dataku.txt digunakan untuk menambahkan izin read, write, dan execute untuk user (pemilik), group, dan others pada file atau direktori dataku.txt.
dan ls -l
Perintah ls -l digunakan untuk melihat izin akses file dan direktori di Linux

## 7. Hapuslah direktori maret. 

<img width="252" alt="100  langkah 7" src="https://github.com/user-attachments/assets/efd3182a-5eed-487c-8d23-3020da279466">

### a. keluar terlebih dahulu dari subdirektori maret dengan cd .. untuk pindah ke direktori induk dari direktori saat ini.
### b. Perintah rm -r maret digunakan untuk menghapus direktori bernama maret beserta seluruh isinya 
### c. ls Perintah ls digunakan untuk menampilkan daftar file dan direktori dalam direktori saat ini.


## 8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapatmelakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari.

<img width="392" alt="langkah 8_tugas 04" src="https://github.com/user-attachments/assets/130456f1-e95a-4248-9857-fc49692785de">

### Untuk mengubah kepemilikan (ownership) sebuah file atau direktori menjadi root, Anda dapat menggunakan perintah chown.

<img width="280" alt="langkah 8_part 2_tugas 04" src="https://github.com/user-attachments/assets/85a0753a-f84d-4313-9dab-44f7d0ba088c">


### juga bisa menggunakan Perintah chmod 750 digunakan untuk mengatur izin akses pada file atau direktori dengan kode numerik 750
### gunakan mkdir unuk menambah sub direktori haha

### 9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya ? 

<img width="309" alt="Langkah 9_Tugas 04" src="https://github.com/user-attachments/assets/52551dee-dd74-4732-b50e-69e13e499b58">

### umask: Perintah ini digunakan untuk menampilkan nilai umask saat ini. Umask adalah sebuah bilangan yang menentukan izin akses default untuk file dan direktori yang baru dibuat.
### umask 0002: Perintah ini digunakan untuk mengatur nilai umask menjadi 0002. Artinya, ketika pengguna membuat file baru, file tersebut akan memiliki izin baca dan tulis untuk pemilik, baca untuk grup, dan tidak ada izin untuk pengguna lain.
### umask 027: Perintah ini digunakan untuk mengatur nilai umask menjadi 027. Artinya, ketika pengguna membuat file baru, file tersebut akan memiliki izin baca dan tulis untuk pemilik, tidak ada izin untuk grup, dan tidak ada izin untuk pengguna lain.

### 10. . Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ? 
<img width="366" alt="Langkah 10_Tugas 04" src="https://github.com/user-attachments/assets/65136056-00cf-4a04-8482-aa0a152f499b">'

### a. ln -s dataku.txt dataku.ini: Perintah ini membuat link simbolik bernama dataku.ini yang menunjuk ke file dataku.txt. Artinya, ketika Anda mengakses dataku.ini, sebenarnya sedang mengakses isi dari dataku.txt.
### b.ln -s dataku.txt dataku.juga: Perintah ini melakukan hal yang sama, membuat link simbolik dataku.juga yang juga menunjuk ke dataku.txt.
### c.ls: Perintah ini digunakan untuk menampilkan daftar file dan direktori di direktori saat ini.
