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

### Latihan 2

### Program dari latihan 2

![Gambar1](https://github.com/Raihanardiansyah/Labpy03/blob/main/foto/program2.png?raw=true)

### Dan ini untuk hasil dari program tersebut

![Gambar1](https://github.com/Raihanardiansyah/Labpy03/blob/main/foto/hasil2.png?raw=true)

### Berikut penjelasan dari program tersebut

### 1. Deklarasi Modal Awal dan Total Keuntungan

modal_awal = 100_000_000 menetapkan modal awal sebesar 100 juta.

total_keuntungan = 0 menginisialisasi variabel total_keuntungan untuk menyimpan akumulasi keuntungan dari bulan pertama hingga bulan kedelapan.



### 2. Loop untuk Menghitung Keuntungan Setiap Bulan

for bulan in range(1, 9): adalah loop for yang berjalan dari 1 hingga 8 (karena range(1, 9) menghasilkan nilai dari 1 hingga 8), yang mewakili bulan ke-1 hingga bulan ke-8.

### 3. Menghitung Keuntungan Berdasarkan Bulan

Di dalam loop, terdapat beberapa kondisi if-elif untuk menentukan besaran keuntungan pada setiap bulan:

Bulan 1 dan 2: if bulan in [1, 2] - Belum ada keuntungan, jadi keuntungan = 0.

Bulan 3 dan 4: elif bulan in [3, 4] - Mulai mendapat keuntungan 1% dari modal awal, jadi keuntungan = modal_awal * 0.01.

Bulan 5, 6, dan 7: elif bulan in [5, 6, 7] - Keuntungan meningkat menjadi 5% dari modal awal, jadi keuntungan = modal_awal * 0.05.

Bulan 8: elif bulan == 8 - Keuntungan menurun menjadi 3% dari modal awal, jadi keuntungan = modal_awal * 0.03.

### 4. Menambahkan Keuntungan ke Total Keuntungan

total_keuntungan += keuntungan menambahkan nilai keuntungan yang diperoleh di bulan tersebut ke total_keuntungan.

### 5. Mencetak Keuntungan Bulanan

print(f"laba bulan ke-{bulan} sebesar: {keuntungan}") menampilkan keuntungan setiap bulan sesuai urutan.

6. Menampilkan Total Keuntungan Setelah 8 Bulan

Setelah loop selesai, print(f"Total laba adalah: {total_keuntungan}") menampilkan total keuntungan yang diperoleh selama 8 bulan.

### Alur Eksekusi

Program mulai dengan modal awal sebesar 100 juta dan menghitung keuntungan setiap bulan selama 8 bulan.

Berdasarkan ketentuan keuntungan setiap bulan, program menambah keuntungan bulanan ke total_keuntungan.

Program mencetak keuntungan setiap bulan dan, pada akhirnya, mencetak total keuntungan setelah 8 bulan.

### Output Contoh

Output program ini akan sesuai dengan aturan yang diberikan:

laba bulan ke-1 sebesar: 0

laba bulan ke-2 sebesar: 0

laba bulan ke-3 sebesar: 1000000.0

laba bulan ke-4 sebesar: 1000000.0

laba bulan ke-5 sebesar: 5000000.0

laba bulan ke-6 sebesar: 5000000.0

laba bulan ke-7 sebesar: 5000000.0

laba bulan ke-8 sebesar: 3000000.0

Total laba adalah: 19000000.0

### Rincian Keuntungan Bulanan

Bulan 1 & 2: Tidak ada keuntungan.

Bulan 3 & 4: 1% dari 100 juta = 1 juta per bulan.

Bulan 5, 6 & 7: 5% dari 100 juta = 5 juta per bulan.

Bulan 8: 3% dari 100 juta = 3 juta.

### Total keuntungan selama 8 bulan = 19 juta.

### Latihan 3

### Program dari latihan 3

![Gambar1](https://github.com/Raihanardiansyah/Labpy03/blob/main/foto/program3.png?raw=true)

### Dan ini untuk hasil dari program tersebut

![Gambar1](https://github.com/Raihanardiansyah/Labpy03/blob/main/foto/hasil3.png?raw=true)

### Berikut penjelasan dari prongram tersebut:

Program ini adalah simulasi sederhana dari sebuah mesin ATM yang memiliki dua opsi: untuk menarik uang atau keluar dari program. Berikut adalah penjelasan kode program ini:

### 1. Inisialisasi Saldo:

saldo = 1000000

Variabel saldo diset awalnya dengan nilai 1.000.000, yang merepresentasikan saldo awal pada akun pengguna.

### 2. Fungsi tampilkan_menu():

Fungsi ini menampilkan menu kepada pengguna dengan pilihan untuk "Tarik Uang" atau "Keluar". Fungsi ini juga menampilkan saldo saat ini.

### 3. Loop while True:

Program berjalan dalam loop while True, yang berarti akan terus berjalan hingga pengguna memilih untuk keluar.


### 4. Input Pilihan Pengguna:

Pengguna diminta untuk memasukkan pilihan mereka, yaitu "1" untuk tarik uang atau "2" untuk keluar.

### 5. Logika Pilihan:

Jika Pilihan "1" (Tarik Uang):

Pengguna akan diminta memasukkan jumlah uang yang ingin ditarik.

Validasi:

Jika jumlah yang diminta lebih besar dari saldo, program akan menampilkan pesan "Saldo tidak cukup!".

Jika jumlah kurang dari atau sama dengan 0, program akan menampilkan "Jumlah penarikan tidak valid!".

Jika valid, saldo akan dikurangi dengan jumlah yang ditarik, dan menampilkan pesan "Penarikan berhasil!".

Jika input bukan angka (misalnya huruf), program akan menangkap ValueError dan menampilkan "Input tidak valid! Masukkan angka."

Jika Pilihan "2" (Keluar):

Program akan menampilkan pesan "Terima kasih telah menggunakan ATM!" dan mengakhiri loop dengan break.

Jika Pilihan Tidak Valid:

Jika input pilihan tidak sama dengan "1" atau "2", program akan menampilkan "Pilihan tidak valid! Silakan coba lagi."
