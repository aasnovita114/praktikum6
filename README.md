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


Lab 3 Perulangan
Latihan 1
Buat program dengan perulangan bertingkat (nested) for yang menghasilkan output sebagai berikut : 200156779-cc2eb0c1-293c-4089-84d8-7dde04482340
Langkah - langkah :

Buat programnya terlebih dahulu seperti gambar di bawah ini



for i in range(0,10):
    print()
    print(i, end="\t")
    for j in range(1,10):
        print(i+j,end="\t")
Hasil Run
Screenshot (127)

Latihan 2
Tampilkan n bilangan acak yang lebih kecil dari 0.5.

Nilai n diisi pada saat runtime

Anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya

Langkah - langkah :

Buatlah programnya terlebih dahulu seperti gambar dibawah ini
Screenshot (128)

from random import random

n = int(input("Masukan Beberapa perulangan : "))
while n == n:
    break
for i in range(n):
    bil = random() % 0.5
    print("Perulangan ke : ", bil)
Hasil Run
Screenshot (129)

MODUL PRAKTIKUM 2 DAN 3
Labpy2 dan Labpy3
Labpy2
Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan tersebut tampilkan bilangan terbesarnya. Gunakan statement if.
Langkah - langkah :

Buatlah flowchart dari mencari angka terbesar dari 3 bilangan seperti gambar dibawah ini
200159462-6b7e6bcb-8a43-4d48-a4c4-5bf8bda85a42

Buatlah program codenya seperti gambar dibawah ini
Screenshot (130)

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
Screenshot (131)

Labpy3
Latihan 1
Flowchart latihan 1

200159707-ccb1abdb-be69-4849-96c8-6c02c439d199

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
Screenshot (132)

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
Screenshot (133)

Latihan 2
Flowchart latihan 2

200159970-42dd1c12-2af8-416d-b808-822ed3c3c7fc

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
Screenshot (134)

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
Screenshot (135)

Program 1
Flowchart program 1

200160200-2f3db728-7d3d-48c0-b21a-b8d3bf11438b

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
Screenshot (136)

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
Screenshot (137)

Sekian, Terima kasih
