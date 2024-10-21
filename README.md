# Praktikum 3 - Tipe Data, Variable, dan Operator

Nama : muflih

Kelas : TI.24.A.5

NIM : 312410527

Mata Kuliah : Bahasa Pemograman


## Mencari bilangan terbesar dari bilangan yang diinputkan
Program ini menentukan bilangan terbesar dari serangkaian bilangan yang diinputkan hingga input 0. Program ini menggunakan loop `while` dan kondisi `if` untuk memperbarui nilai terbesar yang ditemukan.

## Flowchart Program
![Foto](![fc 2,3](https://github.com/user-attachments/assets/fa62791c-8109-4357-a964-92fff95399d6)
)

## kode Program
```python
maxBilangan = float('-inf')  # -∞
count = 0

while True:
    print("Masukkan bilangan (0 untuk berhenti):")
    bilangan = int(input())  

    if bilangan == 0:
        break  

    if bilangan > maxBilangan:
        maxBilangan = bilangan  

    count += 1 


if count > 0:
    print("Bilangan terbesar adalah:", maxBilangan)
else:
    print("Tidak ada bilangan yang dimasukkan.")

```
## penjelasan kode program

```python
maxBilangan = float('-inf')  # -∞
count = 0
```
`maxBilangan` diinisialisasi dengan minus tak hingga (`-∞`). Ini dilakukan agar bilangan pertama yang dimasukkan selalu lebih besar dan bisa menggantikan nilai awal tersebut.
`count` digunakan untuk menghitung jumlah bilangan valid yang dimasukkan.

```python
while True:
    print("Masukkan bilangan (0 untuk berhenti):")
    bilangan = int(input())  # Input bilangan
```
Loop `while` True akan terus berjalan hingga pengguna memasukkan `0`.
Setiap kali loop berjalan, pengguna diminta memasukkan bilangan melalui `input()`.
Input dari pengguna dikonversi ke integer menggunakan `int()`.
