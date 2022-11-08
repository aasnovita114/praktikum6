# Tugas 7

Nama : Aas novitasari

NIM : 312210167

Kelas : TI.22.A1

KONDISI DAN PERULANGAN
Lab 2 Struktur Kondisi
Latihan 1
Buat program sederhana dengan input 2 buah bilangan, kemudian tentukan bilangan terbesar dari kedua bilangan tersebut menggunakan statement if!
Langkah - langkah :

Buat programnya terlebih dahulu seperti gambar di bawah ini
![1](https://user-images.githubusercontent.com/116045324/200510424-3d0b51d6-6831-4eb0-a87e-ba824a0f321c.PNG)

# menentukan bilangan
print('Menentukan bilangan terbesar dari 2 bilangan')
a = int(input("Masukkan nilai A:"))
b = int(input("Masukkan nilai B:"))
if a > b:
    print("A =", a, "yang terbesar")
elif b > a:
    print("B=", b, "yang terbesar")
Hasil Run
![2](https://user-images.githubusercontent.com/116045324/200510689-e1554b83-9946-447a-8778-a01d1f4dc811.PNG)


Latihan 2
Buat program untuk mengurutkan data berdasarkan input sejumlah data (minimal 3 variable input atau lebih), kemudian tampilkan hasilnya secara berurutan mulai dari data terkecil.
Langkah - langkah :
![3](https://user-images.githubusercontent.com/116045324/200511428-f2806cde-237b-4e5d-afe1-35986d3df740.PNG)

Buat programnya terlebih dahulu seperti gambar di bawah ini


print("_____Mengurutkan bilangan dari yang terkecil ke yang terbesar_____")
print("Masukan 3 bilangan yang akan diurutkan:")
a = int(input("masukkan bilangan 1 = "))
b = int(input("masukkan bilangan 2 = "))
c = int(input("masukkan bilangan 3 = "))

if a < b and a < c:
    if b < c:
        print(a, b, c)
    else:
        print(a, c, b)
elif b < a and b < c:
    if a < c:
        print(b, a, c)
    else:
        print(b, c, a)
else:
    if a < b:
        print(c, a, b)
    else:
        print(c, b, a)
Hasil Run
![4](https://user-images.githubusercontent.com/116045324/200519552-b1709006-1b63-4fcd-a104-2221135fdc37.PNG)



Lab 3 Perulangan
Latihan 1
Buat program dengan perulangan bertingkat (nested) for yang menghasilkan output sebagai berikut :
Langkah - langkah :

Buat programnya terlebih dahulu seperti gambar di bawah ini
![lab3 py latihan1](https://user-images.githubusercontent.com/116045324/200520452-74326b77-af0a-4809-984c-a0159e696c55.PNG)



for i in range(0,10):
    print()
    print(i, end="\t")
    for j in range(1,10):
        print(i+j,end="\t")
Hasil Run
![hasilrunlab3latihan1](https://user-images.githubusercontent.com/116045324/200520597-5769bd94-f4cf-4f7b-bc04-7b82a7ae8223.PNG)


Latihan 2
Tampilkan n bilangan acak yang lebih kecil dari 0.5.

Nilai n diisi pada saat runtime

Anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya

Langkah - langkah :

Buatlah programnya terlebih dahulu seperti gambar dibawah ini
![lab3 py latihan2](https://user-images.githubusercontent.com/116045324/200520886-50161ce9-7cb8-4059-b746-0706ac1436f6.PNG)

from random import random

n = int(input("Masukan Beberapa perulangan : "))
while n == n:
    break
for i in range(n):
    bil = random() % 0.5
    print("Perulangan ke : ", bil)
Hasil Run
![hasilrunlab3latihan2](https://user-images.githubusercontent.com/116045324/200521026-8c907426-594b-4fca-94e1-1b99fa04a3f2.PNG)


MODUL PRAKTIKUM 2 DAN 3
Labpy2 dan Labpy3
Labpy2
Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan tersebut tampilkan bilangan terbesarnya. Gunakan statement if.
Langkah - langkah :

Buatlah flowchart dari mencari angka terbesar dari 3 bilangan seperti gambar dibawah ini
![image](https://user-images.githubusercontent.com/116045324/200526475-7eaacb57-4c18-4af6-bc1f-e01605c6c90c.png)


Buatlah program codenya seperti gambar dibawah ini
![5](https://user-images.githubusercontent.com/116045324/200522497-3740e197-c79b-4798-a892-8dec1d08226f.PNG)

a, b, c = (
    int(input('Masukkan nilai a: ')),
    int(input('Masukkan nilai b: ')),
    int(input('Masukkan nilai c: '))
)
if a > b and a > c:
    print('A yang terbesar')
elif b > a and b > c:
    print('B yang terbesar')
else:
    print('C yang terbesar')
Hasil Run
![6](https://user-images.githubusercontent.com/116045324/200522937-4d700c63-4ff5-455b-a67e-941f613797a6.PNG)


Labpy3
Latihan 1
Flowchart latihan 1
![image](https://user-images.githubusercontent.com/116045324/200526864-a34e40e2-0ea1-4fbd-9e82-cde0cb131166.png)



Algoritma latihan 1
Menampilkan n bilangan acak yang lebih kecil dari 0,5, nilai n diisi pada saat runtime.

Memasukan/ import fungsi RANDOM terlebih dahulu

Deklarasi integer , masukkan jumlah n :

Memasukan deskripsi kombinasi for untuk menyelesaikannya.

Memasukan nilai jumlah (n) : 5

Mencetak data ke 1 sampai 5 dengan hasil nilai kurang dari 0,5.

Selesai

Langkah - langkah :

Buat program codenya seperti gambar dibawah ini
![7](https://user-images.githubusercontent.com/116045324/200523208-c3820859-650b-4d6b-859a-cd5c12ee2746.PNG)


print("bilangan acak yang lebih kecil dari o.5")
import random

n = int(input("masukan nilai:"))
a = 0
for c in range(n):
    a += 1
    b = random.uniform(.0, .5)
    print("data ke:", a, "==>", b)

print("selesai")
Hasil Run
![8](https://user-images.githubusercontent.com/116045324/200523372-1984262d-7619-4b9b-9a26-3899377ce3ff.PNG)


Latihan 2
Flowchart latihan 2
![image](https://user-images.githubusercontent.com/116045324/200527044-7a88c7b5-044a-4e47-9cbc-8d23cc3dcb1d.png)



Algoritma latihan 2
Membuat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan.Masukkan angka 0 untuk berhenti

Mulai

Mencetak "latihan 2"

Mencetak "menampilkan bilangan, berhenti ketika bilangan 0, menampilkan bilangan terbesar"

integer max = 0

Menggunakan fungsi perulangan while true, hingga menampilkan perulangan sampai batas tertentu.

Memasukan bilangan integer pada "a"

Menggunakan fungsi if jika max kurang dari nilai a, maka max sama dengan a

Mengunakan fungsi if jika nilai a adalah 0 maka fungsi break artinya perulangan berhenti jika menulis nilai 0.

Mencetak nilai paling terbesarv setelah break, sehingga menampilkan nilai terbesar diantara bilangan tersebut dalam perulangan.

Selesai

Langkah - langkah :

Buatlah program code seperti gambar dibawah ini
![9](https://user-images.githubusercontent.com/116045324/200524127-5558074c-5aed-41e8-9e23-fe5548916935.PNG)


print("menampilkan bilangan, berhenti ketika bilangan 0, dan menampilkan bilangan terbesar")

max = 0
while True:
    angka = int(input("masukan bilangan : "))
    if max < angka:
        max = angka
    if angka == 0:
        break
print("bilangan terbesarnya adalah = ", max)
print("======selesai======")
Hasil Run
![10](https://user-images.githubusercontent.com/116045324/200524618-834e842d-d0b2-49ae-bc10-3705709eaf91.PNG)


Program 1
Flowchart program 1
![image](https://user-images.githubusercontent.com/116045324/200527219-63ac7348-c657-4ecd-ab06-9c2138c106b9.png)



Algoritma dari program 1
Mulai

Mencetak latihan1

Mencetak "Program menghitung laba dengan modal awal 100 juta"

Membuat Note

Mencetak Bulan pertama dan kedua = 0%

Mencetak bulan ke 3 = 1%

Mencetak bulan ke 5 = 5%

Mencetak bulan ke 8 = 2%

integer a = 100.000.000( modal awal)

Menggunakan fungsi looping for pada nilai x 1-9 untuk menampilkan bulan 1 sampai bulan 8.

Menggunakan fungsi if, untuk menghitung laba bulan 1 sampai 8

bulan pertama dan kedua laba adalah 0

bulan ke 3 dan ke 4 mendapat laba 1% sehingga modal di kali 1% = keuntungan

bulan ke 5 mendapatkan laba 5%, sehingga modal dikali 5% = keuntungan

Bulan ke 8 mmendapatkan laba 2% sehingga keuntungan menurun dari bulan sebelumnya, modal dikali 2% = keuntungan.

Menghitung jumlah total laba dengan menjumlah keuntungan dari bulan ke 1 sampai bulan 8, hasilnya adalah total keuntungan yang didapat.

Selesai

Langkah - langkah :

Buatlah program codenya seperti gambar dibawah ini
![11](https://user-images.githubusercontent.com/116045324/200524991-5a13f833-e886-4674-a20e-4264afbec5a2.PNG)


x = 100000000
sum = 0
y = 0
lb = [int(0), int(0), int(x) * .1, int(x) * .1, int(x) * .5, int(x) * .5, 
int(x) * .5, int(x) * .2]
print("modal awal seorang pengusaha :', x")
for i in lb:
    sum = sum + i
    y += 1
    print("#laba bulan ke - ", y, "sebesar :", i)

    print("  TOTAL LABA YANG DIDAPAT ADALAH :", sum)
Hasil Run
![12](https://user-images.githubusercontent.com/116045324/200525198-806bd8a2-ba7f-41d1-93b7-d2943fca5653.PNG)


Sekian, Terima kasih
