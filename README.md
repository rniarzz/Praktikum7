# Nama: Rini Ariza
# NIM: 312210337
# Kelas: TI.22.A3

# PERTEMUAN 11
# Latihan
# Soal

<img width="599" alt="204750979-3c06dc9f-87fd-40b1-8087-ad6efff91c00" src="https://user-images.githubusercontent.com/115542704/205072862-f8fc5e19-eb60-4eb8-bd72-3dea85fcf30a.png">

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

<img width="554" alt="204752446-3289e1d2-7395-4f23-810c-eaa1c4c8323b" src="https://user-images.githubusercontent.com/115542704/205073183-0b606f09-d0fd-4338-ac58-8867f47281e8.png">




