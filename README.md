# Post Test 1 Dasar dasar Pemrograman
## Daftar Isi
* [Identitas](https://github.com/KhalilPradiptaLee/Posttest1DDP#identitas)
* [Penjelasan](https://github.com/KhalilPradiptaLee/Posttest1DDP#penjelasan)
  * [Flow Chart](https://github.com/KhalilPradiptaLee/Posttest1DDP#flow-chart)
  * [Screenshot Input dan Output](https://github.com/KhalilPradiptaLee/Posttest1DDP#screenshot-input-dan-output)
  * [Penjelasan Output](https://github.com/KhalilPradiptaLee/Posttest1DDP#penjelasan-output)
## Identitas
Nama : Khalil Pradipta Lee\
NIM : 2309116046

## Penjelasan
### Flow-chart
![Flowchart Kalk Bangun Ruang -Halaman-1 drawio](https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/83fa9a6c-2cc1-40ae-b56e-03e91bee8055)
![Flowchart Kalk Bangun Ruang -Halaman-2 drawio](https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/f520bdeb-67f2-49a9-a784-4049fb8e1fa2)

## Screenshot Input dan Output
<img width="960" alt="Cuplikan layar 2023-09-25 223554" src="https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/9fb58e40-815a-44d0-a498-268dfab8bcaa">
<img width="960" alt="Cuplikan layar 2023-09-25 223615" src="https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/6bab67a2-ab28-4ee9-8a88-f297587b4116">

### Penjelasan Output

Isi Output :
Pertama-tama, pengguna akan melihat pesan selamat datang
```
Selamat datang di Kalkulator Sederhana!

==========================================
```
Kemudian, program akan meminta pengguna untuk melakukan login dengan menginputkan Nama Mahasiswa, NIM Mahasiswa, dan Password. 
```
Silakan input data pada menu dibawah berikut:
Nama Mahasiswa: (input)
NIM Mahasiswa: (input)
Password: (input)
```
Kode program akan memeriksa apakah NIM hanya berisi angka dan memberi pesan kesalahan jika NIM tidak memenuhi kriteria. Jika semua informasi benar, program akan berlanjut menuju menu berikutnya.
```
Silakan input data pada menu dibawah berikut:
Nama Mahasiswa: Khalil Pradipta Lee
NIM Mahasiswa: 2309116046
Password: testing
Selamat Datang kembali: Khalil Pradipta Lee !
```
Ketika input NIM menggunakan selain angka maka akan terjadi error dan kembali pada bagian login kembali.
```
Nama Mahasiswa: Khalil Pradipta Lee
NIM Mahasiswa: dua tiga nol sembilan
NIM hanya boleh berisi angka. Silakan coba lagi.
Silakan input data pada menu dibawah berikut:
Nama Mahasiswa:
```

Pengguna dapat memilih salah satu opsi dengan memasukkan angka yang sesuai (1, 2, 3, atau 4). Bergantung pada pilihan pengguna, program akan menjalankan fungsi yang sesuai untuk menghitung volume bola, tabung, atau limas segitiga, atau melakukan logout.
```
Menu Pilihan:
============
1. Bola
2. Tabung
3. Limas Segitiga
4. Logout
============
Pilih opsi (1/2/3/4):
```
Ketika input selain dari format tersebut, maka akan terjadi error dan kembali pada menu memilih kembali.
```
Pilih opsi (1/2/3/4): 0
Pilihan tidak valid. Silahkan Ketik Menggunakan format yang telah ada.

Menu Pilihan:
============
1. Bola
2. Tabung
3. Limas Segitiga
4. Logout
============
Pilih opsi (1/2/3/4):
```
Masuk pada bagian kalkulator bangun ruang, kita tinggal menginputkan angka yang kita pilih dan kemudian akan diproses otomatis oleh program dan setelah hasilnya keluar akan kembali ke menu memilih kembali.
```
Menu Pilihan:
============
1. Bola
2. Tabung
3. Limas Segitiga
4. Logout
============
Pilih opsi (1/2/3/4): 1
Masukkan jari-jari bola: 50
Volume bola adalah : 523333.33
```

Jika input angka <= 0 maka akan terjadi error dan akan kembali ke menu memilih.
```
Menu Pilihan:
============
1. Bola
2. Tabung
3. Limas Segitiga
4. Logout
============
Pilih opsi (1/2/3/4): 1
Masukkan jari-jari bola: 0
Nilai jari-jari bola tidak boleh kurang dari atau sama dengan 0.

Menu Pilihan:
============
1. Bola
2. Tabung
3. Limas Segitiga
4. Logout
============
Pilih opsi (1/2/3/4): 1
Masukkan jari-jari bola: -5
Nilai jari-jari bola tidak boleh kurang dari atau sama dengan 0.
```

Jika pengguna memilih input logout maka program akan berakhir dan tertutup.
```
Menu Pilihan:
============
1. Bola
2. Tabung
3. Limas Segitiga
4. Logout
============
Pilih opsi (1/2/3/4): 4
Logout Berhasil, Khalil Pradipta Lee!

Terima kasih telah menggunakan aplikasi ini. Selamat tinggal!
```
