# Nama: Rini Ariza
# NIM: 312210337
# Kelas: TI.22.A3

# Latihan

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
