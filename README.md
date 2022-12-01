# Nama: Rini Ariza
# NIM: 312210337
# Kelas: TI.22.A3

# PERTEMUAN 11
# Latihan
# Soal

![Gambar WhatsApp 2022-12-01 pukul 20 59 46](https://user-images.githubusercontent.com/115542704/205072115-e6e81a4c-a756-45a9-8a85-f736149f7c3e.jpg)

Masukan input sebagai berikut:

```python
telepon = {
    'Thor' : '086969969',
    'Loki' : '08234562'
}

print(telepon['Thor'])

print("\n")

telepon['Heimdal'] = '0813345643'
telepon['Surtr'] = '0824574123'

print(telepon.keys())
print(telepon.values())

print("\n")

print("Nama\t| Nomor Telepon ")
print("======================")

for nama,nomor in telepon.items():
    print("%s \t| %s " % (nama,nomor))

print("\n")

del telepon['Heimdal']

print("Nama\t| Nomor Telepon")
print("======================")
for key,val in telepon.items():
    print("%s \t| %s " % (key,val))
    
```
Maka outputnya akan jadi seperti ini:

<img width="833" alt="ss18" src="https://user-images.githubusercontent.com/115542704/205069437-a1427f27-1ba4-406f-a7a8-8d8c413ee2d1.png">

# Tugas Praktikum
# Soal

![Gambar WhatsApp 2022-12-01 pukul 20 56 49](https://user-images.githubusercontent.com/115542704/205071982-1c73b6dc-e515-4426-907e-3512dd016e5f.jpg)



