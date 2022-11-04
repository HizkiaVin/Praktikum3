#Praktikum3
# Latihan 1
Pada latihan 1 kita akan mempelajari penggunaan end, separator, dan string format pada python.
Kita akan mulai dari **penggunaan end** terlebih dahulu.

![Penggunaan End](https://user-images.githubusercontent.com/116176746/199726369-8bb9da05-d4e3-4be2-9cd1-964da5eb7415.png)

Kita menggunakan end pada huruf ABC sedangkan pada huruf XYZ kita tidak menggunakan, maka output yang akan ditampilkan adalah sebagai berikut

![Penggunaan End(1)](https://user-images.githubusercontent.com/116176746/199726379-85cb36de-0932-4b07-b7e8-ec1501be4431.png)
>Parameter end berfungsi untuk mengganti karakter terakhir bawaan yang dicetak di layar.
Jadi secara bawaan, setiap kali kita memanggil fungsi print() untuk mencetak sesuatu, python akan mencetak karakter ganti baris (\n) di setiap output.

Setelah itu kita akan mempelajari **penggunaan separator**

![Penggunaan Separator ](https://user-images.githubusercontent.com/116176746/199969672-fa3eb478-da6e-4f98-bee0-d1987b504ff1.png)

Pada perintah print() pertama tanpa parameter sep, sehingga python otomatis menjadikan karakter spasi sebagai pemisah.
Sedangkan perintah print() yang selanjutnya, saya menggunakan parameter sep dengan nilai (,)('')(:) dan (----), maka output yang akan dihasilkan adalah sebagai berikut

![Penggunaan Separator (1)](https://user-images.githubusercontent.com/116176746/199969684-15e53d08-5c12-4d2b-8f4a-f5400fc52928.png)


>Ketika kita memanggil fungsi print() untuk menampilkan multi argumen, python akan otomatis menambahkan karakter spasi sebagai pemisah antar argumen tersebut.
Jika kita tidak ingin pemisah spasi, maka kita bisa menambahkan parameter sep (separator) saat memanggil print().

**String Format**


![String Format](https://user-images.githubusercontent.com/116176746/199974914-472769c4-d84d-4f42-8ff2-5c29a94a30d3.png)

Outputnya adalah : 

![String Format (1)](https://user-images.githubusercontent.com/116176746/199974923-02c2e5dd-95ce-4447-bec0-f8d56cf31d1c.png)

>nilai yang diformat mengambil lebar sebanyak karakter yang akan direpresentasikannya. Akan tetapi, kita bisa mengatur sendiri berapa lebar yang kita inginkan. Kita bisa menggunakan perintah **'{:>10}'.format('test')**

# Latihan 2
![Konversi nilai variable](https://user-images.githubusercontent.com/116176746/199982751-d0826160-716f-4904-9b18-9e51d1103bfe.png)

>a=input("masukkan nilai a:")
b=input("masukkan nilai b:")

print("variable a=",a)
print("variable b=",b)
print("hasil penggabungan {1}&{0}=%s".format(a,b) %(a+b))

#konversi nilai variable
a=int(a)
b=int(b)
print("hasil penjumlahan {1}+{0}=%d".format(a,b) %(a+b))
print("hasil pembagian {1}/{0}=%d".format(a,b) %(a/b))
