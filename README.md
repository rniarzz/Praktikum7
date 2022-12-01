# Nama: Rini Ariza
# NIM: 312210337
# Kelas: TI.22.A3

## PERTEMUAN 11
## Latihan
## Soal

<img width="599" alt="204750979-3c06dc9f-87fd-40b1-8087-ad6efff91c00" src="https://user-images.githubusercontent.com/115542704/205072862-f8fc5e19-eb60-4eb8-bd72-3dea85fcf30a.png">

## Jawab

Masukan input sebagai berikut:

```python
import math
def a(x):
  return x**2
a = lambda x : x**2
print(a(2))
def b(x, y):
  return math.sqrt(x**2 + y**2)
b = lambda x, y : x ** 2 + y ** 2
print(b(2, 2))
def c(*args):
  return sum(args)/len(args)
c = lambda *args : sum(args)/len(args)
print(c(1,2,3,4,5))
def d(s):
  return "".join(set(s))
d = lambda s: "".join(set(s))
print(d("buku"))
```
## Output:

<img width="419" alt="ss 19" src="https://user-images.githubusercontent.com/115542704/205075086-b76c06e6-e36b-4a6e-bf78-888d71113dfd.png">

# Tugas Praktikum
# Soal

<img width="554" alt="204752446-3289e1d2-7395-4f23-810c-eaa1c4c8323b" src="https://user-images.githubusercontent.com/115542704/205073183-0b606f09-d0fd-4338-ac58-8867f47281e8.png">

## Jawab

- Pertama buat dahulu **dictionary** kosong untuk menampung data-data yang ingin diinputkan
```python
mahasiswa = {}
```
- Untuk membuat fungsi, dalam python sebuah fungsi didefinisikan menggunakan kata kunci `def ():`
- Untuk program menambah data kita gunakan fungsi `def tambah():`, berikut programnya:
```python
def tambah():
    print("Tambah Data")
    nama = input("Masukkan Nama Mahasiswa   : ")
    nim = input("Masukkan NIM              : ")
    tugas = int(input("Masukkan Nilai Tugas      : "))
    uts = int(input("Masukkan Nilai UTS        : "))
    uas = int(input("Masukkan Nilai UAS        : "))
    akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
    x[nama] = nim , tugas, uts , uas , akhir
```

- Untuk program menampilkan data kita gunakan fungsi `def tampilkan ():`
- Lalu saya membuat format `if else` untuk membuat 2 kondisi, dimana `if` disini digunakan untuk menampilkan data-data dalam tabel yang sudah diinputkan, sedangkan `else` disini digunakan untuk menampilkan sebuah tabel yang belum diinputkan data-data
```python
def tampilkan():
    if x.items():
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        i = 0                                                                         
        for b in x.items():                                                             
             i += 1
             print("| {no:2d} | {0:14s} | {1:11s} | {2:7d} | {3:7d} | {4:7d} | {5:7f}   |"
                . format ( b [ 0 ][: 14 ], b [ 1 ][ 0 ], b [ 1 ][ 1 ], b [ 1 ][ 2 ], b [ 1 ][ 3 ], b [ 1 ][ 4 ] , no = i ))
        print("---------------------------------------------------------------------------------")
    else :
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        print("|                                TIDAK ADA DATA                                 |")
        print("---------------------------------------------------------------------------------")
```
























## Output:
ini adalah output apabila memilih tambah (t)

<img width="286" alt="t 1" src="https://user-images.githubusercontent.com/115542704/205082552-70bec59a-8461-4c07-90b8-f399bfb025fa.png">

ini adalah output apabila memilih lihat (l)

<img width="500" alt="l 1" src="https://user-images.githubusercontent.com/115542704/205083193-7ed44a8e-f683-43df-b603-e859cad1ac4c.png">

ini adalah output apabila memilih ubah (u)

<img width="509" alt="u 1" src="https://user-images.githubusercontent.com/115542704/205083267-70606bc7-7a04-4ae9-bd38-71cf8af96ada.png">

ini adalah output apabila memilih hapus (h) 

<img width="505" alt="h 1" src="https://user-images.githubusercontent.com/115542704/205082847-cf36fc1a-aff2-4598-a7ea-b2436865f68c.png">

ini adalah output apabila memilih keluar (k)

<img width="507" alt="k 1" src="https://user-images.githubusercontent.com/115542704/205082898-e0889652-108c-4b10-b7f7-ca26bd1590fc.png">

## SEKIAN TERIMAKASIH



