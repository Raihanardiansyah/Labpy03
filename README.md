# LAPORAN PRAKTIKUM 3

## Tugas Pertemuan 7

### Latihan 1

### ini adalah progam dari latihan pertama 

![Gambar1](https://github.com/Raihanardiansyah/Labpy03/blob/main/foto/program1.png?raw=true)

### ini hasil dari program tersebut

![Gambar1](https://github.com/Raihanardiansyah/Labpy03/blob/main/foto/hasil1.png?raw=true)

### dan berikut adalah penjelasannya

Berikut adalah penjelasan dari program pertama yang diminta:

Program

from random import random

### Meminta pengguna untuk memasukkan nilai N

n = int(input("Masukkan nilai N: "))

### Inisialisasi variabel penghitung
count = 0

### Loop while untuk memastikan kita mendapatkan N angka acak yang lebih kecil dari 0.5
while count < n:

    # Menghasilkan bilangan acak dan menampilkannya jika kurang dari 0.5
    
    angka_acak = random()
    
    if angka_acak < 0.5:
    
        count += 1
        
        print(f"data ke-{count} => {angka_acak}")

print("Selesai")

Penjelasan Kode

1. Import Modul random

2. from random import random mengimpor fungsi random() dari modul random, yang memungkinkan kita menghasilkan angka acak antara 0 dan 1.

3. Meminta Input Pengguna

n = int(input("Masukkan nilai N: ")) meminta pengguna untuk memasukkan jumlah bilangan acak yang ingin ditampilkan. Nilai ini kemudian disimpan di variabel n.


4. Inisialisasi Variabel count

count = 0 adalah variabel yang akan digunakan untuk menghitung jumlah bilangan acak yang dihasilkan dan memenuhi syarat (< 0.5). Variabel ini memastikan kita mendapatkan tepat n angka acak yang kurang dari 0.5.


5. Loop while untuk Mendapatkan n Angka Acak

while count < n berarti loop akan terus berjalan selama jumlah angka acak yang memenuhi syarat (kurang dari 0.5) masih kurang dari n.


6. Menghasilkan Angka Acak

angka_acak = random() menghasilkan angka acak antara 0 dan 1. Setiap kali loop berjalan, program menghasilkan angka acak baru.


7. Pengecekan Kondisi Angka Acak

if angka_acak < 0.5 mengecek apakah angka acak yang dihasilkan kurang dari 0.5. Jika ya:

count += 1 menambah count sebesar 1, mencatat bahwa kita telah mendapatkan satu angka yang memenuhi syarat.

print(f"data ke-{count} => {angka_acak}") menampilkan angka acak tersebut, dengan format yang menunjukkan urutan ke berapa angka tersebut didapatkan.


Jika angka acak tidak kurang dari 0.5, maka continue digunakan secara implisit karena tidak ada aksi lebih lanjut di dalam loop; program akan kembali ke awal loop untuk menghasilkan angka acak baru.


8. Menampilkan Pesan Akhir

Setelah mendapatkan n angka yang memenuhi syarat, loop while berhenti, dan program menampilkan "Selesai" sebagai tanda bahwa proses telah selesai.

### Alur Eksekusi

Program meminta input jumlah n.

Menghasilkan angka acak hingga mencapai n angka yang memenuhi syarat < 0.5.

Setiap angka yang memenuhi syarat ditampilkan, dan setelah n angka tercapai, program selesai.
