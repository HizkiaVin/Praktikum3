#Praktikum3
# Latihan 1
Pada latihan 1 kita akan mempelajari penggunaan end, separator, dan string format pada python.
Kita akan mulai dari **penggunaan end** terlebih dahulu.
```python
#Penggunaan End
print('A', end='')
print('B', end='')
print('C', end='')
print()
print('X')
print('Y')
print('Z')
```

Kita menggunakan end pada huruf ABC sedangkan pada huruf XYZ kita tidak menggunakan, maka output yang akan ditampilkan adalah sebagai berikut

![Penggunaan End(1)](https://user-images.githubusercontent.com/116176746/199726379-85cb36de-0932-4b07-b7e8-ec1501be4431.png)
>Parameter end berfungsi untuk mengganti karakter terakhir bawaan yang dicetak di layar.
Jadi secara bawaan, setiap kali kita memanggil fungsi print() untuk mencetak sesuatu, python akan mencetak karakter ganti baris (\n) di setiap output.

Setelah itu kita akan mempelajari **penggunaan separator**
```python
#Penggunaan Separator
w, x, y, z = 10, 15, 20 ,25
print(w, x, y, z)
print(w, x, y, z, sep=',')
print(w, x, y, z, sep='')
print(w, x, y, z, sep=':')
print(w, x, y, z, sep='-----')
```
Pada perintah print() pertama tanpa parameter sep, sehingga python otomatis menjadikan karakter spasi sebagai pemisah.
Sedangkan perintah print() yang selanjutnya, saya menggunakan parameter sep dengan nilai (,)('')(:) dan (----), maka output yang akan dihasilkan adalah sebagai berikut

![Penggunaan Separator (1)](https://user-images.githubusercontent.com/116176746/199969684-15e53d08-5c12-4d2b-8f4a-f5400fc52928.png)

>Ketika kita memanggil fungsi print() untuk menampilkan multi argumen, python akan otomatis menambahkan karakter spasi sebagai pemisah antar argumen tersebut.
Jika kita tidak ingin pemisah spasi, maka kita bisa menambahkan parameter sep (separator) saat memanggil `print()`.

**String Format**
```python
#String Format
print(0, 10**0)
print(1, 10**1)
print(2, 10**2)
print(3, 10**3)
print(4, 10**4)
print(5, 10**5)
print(6, 10**6)
print(7, 10**7)
print(8, 10**8)
print(9, 10**9)
print(10, 10**10)

#String Format
print('{0:>3} {1:>16}' .format(0, 10**0))
print('{0:>3} {1:>16}' .format(0, 10**1))
print('{0:>3} {1:>16}' .format(0, 10**2))
print('{0:>3} {1:>16}' .format(0, 10**3))
print('{0:>3} {1:>16}' .format(0, 10**4))
print('{0:>3} {1:>16}' .format(0, 10**5))
print('{0:>3} {1:>16}' .format(0, 10**6))
print('{0:>3} {1:>16}' .format(0, 10**7))
print('{0:>3} {1:>16}' .format(0, 10**8))
print('{0:>3} {1:>16}' .format(0, 10**9))
print('{0:>3} {1:>16}' .format(0, 10**10))

```
Outputnya adalah : 

![String Format (1)](https://user-images.githubusercontent.com/116176746/199974923-02c2e5dd-95ce-4447-bec0-f8d56cf31d1c.png)

>nilai yang diformat mengambil lebar sebanyak karakter yang akan direpresentasikannya. Akan tetapi, kita bisa mengatur sendiri berapa lebar yang kita inginkan. Kita bisa menggunakan perintah **'{:>10}'.format('test')**

# Latihan 2
![Konversi nilai variable](https://user-images.githubusercontent.com/116176746/199982751-d0826160-716f-4904-9b18-9e51d1103bfe.png)

Kita bisa memasukkan perintah sebagai berikut:

```python
a=input("masukkan nilai a:")
b=input("masukkan nilai b:")

print("variable a=",a)
print("variable b=",b)
print("hasil penggabungan {1}&{0}=%s".format(a,b) %(a+b))

#konversi nilai variable
a=int(a)
b=int(b)
print("hasil penjumlahan {1}+{0}=%d".format(a,b) %(a+b))
print("hasil pembagian {1}/{0}=%d".format(a,b) %(a/b))
```

maka outputnya :

![Konversi nilai variable(1)](https://user-images.githubusercontent.com/116176746/199982762-2e18a3e8-5b6b-4921-8f36-53746cac96af.png)


# Latihan 3
![String Formatting(3)](https://user-images.githubusercontent.com/116176746/200011534-edeff368-8ee3-4c7a-b9b7-98a6843c6dec.png)

Untuk menghasilkan output seperti gambar diatas, kita bisa memasukkan kode 

```python
print('{1:>15}'.format(0,"*"))
print('{1:>16}'.format(0,"***"))
print('{1:>17}'.format(0,"*****"))
print('{1:>18}'.format(0,"*******"))
print('{1:>19}'.format(0,"*********"))
print('{1:>18}'.format(0,"*******"))
print('{1:>17}'.format(0,"*****"))
print('{1:>16}'.format(0,"***"))
print('{1:>15}'.format(0,"*"))
```

maka akan menghasilkan output seperti berikut

![String Formatting(1)](https://user-images.githubusercontent.com/116176746/200011539-5457b4da-f646-4ce0-893c-7a93e40e25f2.png)

<hr>

# Tugas

**• Buat kode program untuk menghitung luas dan keliling lingkaran menggunakan Python.**

**• Sertakan flowchart dan penjelasan program dan screenshot hasil
eksekusi program**

![flowchart](https://user-images.githubusercontent.com/116176746/200022135-23605728-fb94-4b5d-89b2-e337f6daac6e.png) 
>Fungsi flowchart adalah menggambarkan alur sebuah program dari setiap prosesnya. Fungsi lainnya, yaitu memampatkan atau menyederhanakan penjelasan dari proses yang ada. Dengan begitu, alir program akan lebih mudah untuk dipahami oleh semua orang.

**Program Menghitung Luas dan Keliling Lingkaran**
```python
import math
r = float (input("Masukkan jari-jari : "))

luas = math.pi  *(r*r)
keliling = 2*math.pi*r

print("Luas lingkaran \t\t= " ,luas)
print("Kelilling lingkaran \t= " ,keliling)
```
>Kita import modul math yang sudah di sediakan oleh python terlebih dahulu. Fungsinya adalah menyertakan nilai phi yang sudah tersedia dalam modul tersebut dengan perintah `math.pi`jika kita coba mencetak fungsi tersebut maka akan menghasilkan nilai 3.14


output nya adalah sebagai berikut

![Tugas](https://user-images.githubusercontent.com/116176746/200028120-1a5d0c7d-e7a0-46d4-a163-0e0940661cb7.png)


# **SELESAI**



