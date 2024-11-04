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
![Foto](https://github.com/nanafnan09/-hasil-foto-kode-pemrograman-labpy03/blob/0b464c038c38070ca092798edc1a3b1af1764fe9/Latihan%201%20b%20pemrograman.png)

# Latihan 2

```
python
modal_awal = 100_000_000
```
Inisialisasi Modal Awal: Baris ini mendefinisikan variabel `modal_awal` dengan nilai 100.000.000 (seratus juta). Ini adalah jumlah modal yang akan digunakan sebagai dasar perhitungan laba.

```
python
laba_bulan = [0, 0, 0.01, 0.01, 0.05, 0.05, 0.05, 0.03]
```
Daftar Persentase Laba Bulanan: Variabel `laba_bulan` adalah sebuah list yang berisi persentase laba untuk setiap bulan. Nilai-nilai dalam list ini adalah:
Bulan 1: 0% (tidak ada laba)
Bulan 2: 0% (tidak ada laba)
Bulan 3: 1%
Bulan 4: 1%
Bulan 5: 5%
Bulan 6: 5%
Bulan 7: 5%
Bulan 8: 3%

```
python
modal = modal_awal
```
Inisialisasi Modal: Variabel `modal` diatur ke nilai `modal_awal`, sehingga perhitungan laba akan dimulai dari jumlah modal awal yang telah ditentukan.

```
python
for i, presentase_laba in enumerate(laba_bulan):
```
Looping Melalui Daftar Laba: Struktur `for` ini digunakan untuk mengiterasi (melakukan loop) melalui daftar `laba_bulan`. Fungsi `enumerate()` memberikan indeks (`i`) dan nilai (`presentase_laba`) untuk setiap elemen dalam list.

```
python
    laba_bulan_ini = modal * presentase_laba
```
Menghitung Laba Bulanan: Di dalam loop, laba untuk bulan ini dihitung dengan mengalikan modal saat ini (`modal`) dengan persentase laba (`presentase_laba`). Hasilnya disimpan dalam `variabel laba_bulan_ini`.

```
python
    modal += laba_bulan_ini
```
Memperbarui Modal: Modal diperbarui dengan menambahkan laba bulan ini ke modal yang ada. Ini mencerminkan pertumbuhan modal berdasarkan laba yang dihasilkan.

```
python
    print(f"laba bulan ke{i+1}: sebesar {presentase_laba*100}& -> Total modal: Rp{modal:,.0f}")
```
Mencetak Hasil: Baris ini mencetak informasi tentang laba bulan ke-i (dengan penambahan satu pada indeks agar dimulai dari bulan pertama) dan total modal saat ini. Format f-string digunakan untuk menyisipkan nilai variabel ke dalam string, dan Rp`{modal:,.0f}` memastikan bahwa total modal ditampilkan dalam format mata uang dengan pemisah ribuan.

```
python
    print(f"\nTotal modal pada akhir bulan ke-8: Rp{modal:,.0f}")
```
Mencetak Total Modal Akhir: Baris ini mencetak total modal pada akhir bulan ke-8 setelah setiap iterasi loop. Namun, perlu dicatat bahwa baris ini seharusnya berada di luar loop jika Anda ingin mencetak total modal hanya sekali setelah semua bulan dihitung.

# Berikut hasil latihan 2
![Foto]()















