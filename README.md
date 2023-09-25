![flowc 1](https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/28f5e23f-cb28-41e7-8442-3ff407149e6c)
![flowc 2](https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/e93d1127-54d7-4cfc-b78d-72c6678c9ad6)
<img width="960" alt="Cuplikan layar 2023-09-25 210954" src="https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/f6cbdf9b-8b85-484a-84b7-5f3ef2a9d7a7">
<img width="960" alt="Cuplikan layar 2023-09-25 211016" src="https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/f0ba3d06-9708-47ab-a948-4df229572059">
<img width="960" alt="Cuplikan layar 2023-09-25 211023" src="https://github.com/KhalilPradiptaLee/Posttest1DDP/assets/144757000/efbc0a17-2a07-4efc-9075-cc3dd5050593">
# Membuat function untuk login, disini terdapat Nama, NIM, dan Password. Setelah melakukan login maka pengguna akan dibawa menuju menu berikutnya yaitu menu pilihan
def login():
    while True: # membuat loop pada login
        print("\nSilakan input data pada menu dibawah berikut:") # \n untuk membuat satu baris kosong ketika program dijalankan
        data_nama = input("Nama Mahasiswa: ") # kita dapat memasukkan nama apapun karena tidak terdapat restriksi pada nama
        
        nim = input("NIM Mahasiswa: ") # NIM hanya dapat menggunakan angka, jadi ketika menggunakan huruf atau yang lainnya akan terjadi error
        if not nim.isdigit(): # .isdigit digunakan untuk cek bahwa NIM hanya menggunakan angka
            print("NIM hanya boleh berisi angka. Silakan coba lagi.")
        else:
            password = input("Password: ")
            print(f"\nSelamat Datang kembali: {data_nama} !")
            return data_nama
            break # keluar dari loop ini dan lanjut ke bagian menu pilihan

# Membuat function untuk membuat rumus bola, tabung, dan limas segitiga terlebih dahulu agar sistem dapat mengetahui isi dari program function jika kita langsung membuat halaman menu maka sistem tidak akan mengetahui isi dari suatu rumus bola, tabung, dan limas segitiga dan terjadi eror

def hitung_volume_bola():
    jari_jari = float(input("Masukkan jari-jari bola: "))
    if jari_jari < 1:
        print("Nilai jari-jari bola tidak boleh dibawah 1.")
    else:
        volume = (4/3) * 3.14 * jari_jari**3 # ** adalah pangkat
        print(f"Volume bola adalah : {volume:.2f}") #.2f agar hasil float yang ditunjukkan hanya 2 bilangan desimal dibelakang angka utama

def hitung_volume_tabung():
    jari_jari = float(input("Masukkan jari-jari tabung: "))
    tinggi = float(input("Masukkan tinggi tabung: "))
    if jari_jari < 1 or tinggi < 1:
        print("Nilai jari-jari/tinggi tabung tidak boleh dibawah 1.")
    else:
        volume = 3.14 * jari_jari**2 * tinggi  # ** adalah pangkat
        print(f"Volume tabung adalah : {volume:.2f}") #.2f agar hasil float yang ditunjukkan hanya 2 bilangan desimal dibelakang angka utama

def hitung_volume_limas_segitiga():
    alas = float(input("Masukkan panjang alas limas segitiga: "))
    tinggisegitiga = float(input("Masukkan tinggi segitiga: "))
    tinggi = float(input("Masukkan tinggi limas segitiga: "))
    if tinggi < 1 or tinggisegitiga < 1 or tinggi < 1:
        print("Nilai alas/tinggi segitiga/tinggi pada limas segitiga tidak boleh dibawah 1.")
    else:
        volume = (1/3) * (1/2 * alas * tinggisegitiga) * tinggi  # ** adalah pangkat
        print(f"Volume limas segitiga adalah : {volume:.2f}") #.2f agar hasil float yang ditunjukkan hanya 2 bilangan desimal dibelakang angka utama

# setelah membuat fungsi rumus-rumus tadi kemudian kita membuat menu utama, di menu utama terdapat 4 pilihan, jika memilih selain dari 4 pilihan tersebut maka akan terjadi eror dan pengguna akan dibawa menuju menu pilihan kembali
def menu_utama(data_nama):
    while True: # membuat loop untuk menu pilihan
        print("\nMenu Pilihan:")
        print("=" * 12) # = * 12 berarti ============
        print("1. Bola")
        print("2. Tabung")
        print("3. Limas Segitiga")
        print("4. Logout") # opsi untuk keluar dari loop menu pilihan sekaligus keluar dari program
        print("=" * 12) # = * 12 berarti ============

# Bagian penginputan data, jika memilih selain dari 4 pilihan tersebut maka akan terjadi eror dan pengguna akan dibawa menuju menu pilihan kembali. Dan jika memilih program sesuai input maka menu akan berlanjut
        pilihan = input("Pilih opsi (1/2/3/4): ")

        if pilihan == "1":
            hitung_volume_bola()
        elif pilihan == "2":
            hitung_volume_tabung()
        elif pilihan == "3":
            hitung_volume_limas_segitiga()
        elif pilihan == "4":
            print(f"Logout Berhasil, {data_nama}!")
            break # agar kita keluar dari loop menu pilihan dan logout sekaligus mengakhiri program
        else:
            print("Pilihan tidak valid. Silahkan Ketik Menggunakan format yang telah ada.")

# ini adalah title ketika kita baru saja menjalankan sebuah program ini. Berfungsi untuk menentukan alur program ini agar runtun
if __name__ == "__main__":
    print("Selamat datang di Kalkulator Sederhana!\n")
    print("=" *42) # = * 12 berarti ============ hingga 42

    while True: # Bagian ini menjalankan program loop tidak terbatas yang memungkinkan kita untuk menjalankan semua program ini secara runtun.
        data_nama = login() # kita harus login terlebih dahulu agar program ini lanjut ke program/fungsi selanjutnya
        menu_utama(data_nama) # Setelah berhasil login, program menjalankan fungsi ini / lanjut ke menu pilihan 
        keluar = print("\nTerima kasih telah menggunakan aplikasi ini. Selamat tinggal!") # akan tercetak setelah kita memilih menu pilihan 4
        exit() # Program berakhir

# Untuk beberapa penjelasan lebih lanjut dapat dilihat dari comment (#) disebelah barisan pemrograman yang telah dibuat
