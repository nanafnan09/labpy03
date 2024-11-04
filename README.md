# Pratikum 3 Perulangan
Nama : Afnan Dika Ramadhan
Kelas : TI24.A5
NIM 312410518

#  Latihan 1

```
python
from random import random
```
Import Modul: Baris ini mengimpor fungsi `random()` `dari modul` `random`, yang digunakan untuk menghasilkan angka acak antara `0.0 dan 1.0.`

```
python
n = int(input("masukan nilai N:"))
```
Input Pengguna: Baris ini meminta pengguna untuk memasukkan nilai `N`, yang kemudian diubah menjadi tipe data integer menggunakan `int()`. Nilai ini menentukan berapa banyak angka acak yang akan dicetak.

```
python
count = 0

```
Inisialisasi Counter: Variabel `count`diinisialisasi dengan `nilai 0`. Variabel ini digunakan untuk menghitung jumlah angka acak yang telah dicetak.

```
python
while count < n:
```
Looping: Struktur kontrol `while` ini akan terus berjalan selama nilai `count` kurang dari `N`. Ini berarti loop akan berjalan sampai kita mencetak `N` angka acak yang memenuhi syarat.

```
python
    random_number = random()
```
Menghasilkan Angka Acak: Di dalam loop, fungsi `random()` dipanggil untuk menghasilkan sebuah angka acak antara 0.0 dan 1.0, dan hasilnya disimpan dalam variabel `random_number`.

```
python
    if random_number < 0.5:
```
Pemeriksaan Kondisi: Baris ini memeriksa apakah `random_number` yang dihasilkan kurang dari 0.5. Jika iya, maka program akan melanjutkan ke langkah berikutnya.

```
python
        print(f" data ke {count} ={random_number}")
```
Mencetak Angka Acak: Jika kondisi sebelumnya terpenuhi, program mencetak angka acak tersebut bersama dengan indeksnya (nilai dari `count`). Format string f-string digunakan di sini untuk menyisipkan nilai variabel ke dalam string.

```
python
        count += 1
```
Increment Counter: Setelah mencetak angka, nilai count ditambah 1. Ini memastikan bahwa kita menghitung jumlah angka yang telah dicetak dan akan menghentikan loop ketika sudah mencapai `N`.


# Berikut hasilnya latihan 1
![Foto]()









