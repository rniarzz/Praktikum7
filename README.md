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
- Untuk program menambah data kita gunakan fungsi `def tambah():`

Berikut programnya:
```python
def tambah():
    print("Tambah Data")
    nama = input("Masukkan Nama Mahasiswa   : ")
    nim = input("Masukkan NIM              : ")
    tugas = int(input("Masukkan Nilai Tugas      : "))
    uts = int(input("Masukkan Nilai UTS        : "))
    uas = int(input("Masukkan Nilai UAS        : "))
    akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
    mahasiswa[nama] = nim , tugas, uts , uas , akhir
```

- Untuk program menampilkan data kita gunakan fungsi `def tampilkan():`
- Lalu saya membuat format `if else` untuk membuat 2 kondisi, dimana `if` disini digunakan untuk menampilkan tabel yang sudah diinputkan data-data sebelumnya, sedangkan `else` disini digunakan untuk menampilkan sebuah tabel yang belum diinputkan data-data

Berikut programnya:
```python
def tampilkan():
    if mahasiswa.items():
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        i = 0                                                                         
        for b in mahasiswa.items():                                                             
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

- Untuk program menghapus data kita gunakan fungsi `def hapus():`

Berikut programnya:
```python
def hapus():
    print ( "Hapus Data" )
    nama = input("Masukkan Nama Mahasiswa   : ")
    if  nama in  mahasiswa . keys ():
        del  mahasiswa [ nama ]
    else :
        print ( "Nama {0} Tidak Ditemukan" . format ( nama ))
```

- Untuk program mengubah data kita gunakan fungsi `def ubah():`

Berikut programnya:
```python
def ubah():
    print ( "Ubah Data" )
    nama = input("Masukkan Nama Mahasiswa   : ")
    if nama in  mahasiswa . keys ():
        nim = input("Masukkan NIM              : ")
        tugas = int(input("Masukkan Nilai Tugas      : "))
        uts = int(input("Masukkan Nilai UTS        : "))
        uas = int(input("Masukkan Nilai UAS        : "))
        akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
        mahasiswa[nama] = nim , tugas, uts , uas , akhir
    else :
        print ( "Nama{0} Tidak Ditemukan" . format(nama ))
```

- Penggunaan **while True**

  **while True** berfungsi untuk mendeteksi jika format yang diinputkan bukan berupa type maka akan muncul error

- Kemudian saya membuat looping agar program terus berjalan, untuk berhentinya gunakan perintah `break` di akhir program while true
- Variable c dideklarasikan untuk inputan daftar menu yang mau dipilih
- Penggunaan **if c.lower()** (Tidak harus menggunakan variable c, jadi kita bebas mau menggunakan variable apapun)

  **if c.lower()** fungsinya apabila user menginputkan dengan huruf besar, maka otomatis akan menjadi huruf kecil sehingga kondisi yang digunakan tercapai

Berikut programnya:
```python
while True:
    print("")
    print("===========================")
    print("|   Program Input Nilai   |")
    print("===========================")
    c = input("L)ihat, T)ambah, U)bah, H)apus, K)eluar: ")
    if c.lower() == "l":
        tampilkan()
    elif c.lower() == "t":
        tambah()
    elif c.lower() == "u":
        ubah()
    elif c.lower() == "h":
        hapus()
    elif c.lower() == "k":
        print()
        print("---------------------------------------------------------------------------------")
        print("                                 PROGRAM TELAH SELESAI                    ")
        print("---------------------------------------------------------------------------------")
        print(35*'=')
        print("Nama\t: Rini Ariza\nKelas\t: TI.22.A3\nNIM\t\t: 312210337")
        print(35*'=')
        break
```

- Dan saya juga menggunakan else di akhir program yang digunakan apabila salah memasukkan pilihan inputan

Berikut programnya:
```python
    else:
        print()
        print("Kode yang anda masukkan salah!")
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

<img width="506" alt="k 3" src="https://user-images.githubusercontent.com/115542704/205201368-4cc2f841-ea90-4a15-9346-46bd84dc328f.png">

## SEKIAN TERIMAKASIH



