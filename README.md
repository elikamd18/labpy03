# **Tugas Praktikum 3 – labpy03**

## Nama : Elika Manuela Damanik  
## Prodi: Teknik Informatika – Universitas Pelita Bangsa  

Latihan 1 – Bilangan Acak Kurang dari 0.5
Kode Program (latihan1.py)
```python
from random import random
n = int(input("Masukkan nilai N: "))
i = 0
while i < n:
    a = random()
    if a < 0.5:
        print(f"data ke: {i+1} => {a}")
        i += 1
print("Selesai")
Alur Algoritma:
1. Program mengimpor fungsi random dari modul random.
2. Pengguna memasukkan jumlah data n.
3. Program menghasilkan bilangan acak dengan fungsi random().
4. Hanya angka yang lebih kecil dari 0.5 yang akan ditampilkan.
5. Program berakhir setelah menampilkan n data, lalu mencetak “Selesai”.
Contoh Output:
Masukkan nilai N: 5
data ke: 1 => 0.1729492204357056
data ke: 2 => 0.08717360127477924
data ke: 3 => 0.05051607654502832
data ke: 4 => 0.27535124215716744
data ke: 5 => 0.39262323000723776
Selesai

---

Latihan 2 – Menghitung Laba Usaha
Kode Program (latihan2.py)
modal = 100000000
total = 0
for i in range(1, 9):
    if i == 1 or i == 2:
        laba = 0
    elif i == 3 or i == 4:
        laba = modal * 0.1
    elif i == 5 or i == 6 or i == 7:
        laba = modal * 0.5
    elif i == 8:
        laba = modal * 0.2
    total += laba
    print(f"laba bulan ke-{i} sebesar: {laba}")
print(f"Total laba adalah: {total}")

Alur Algoritma:
1. Modal awal ditentukan sebesar 100 juta.
2. Perulangan dilakukan selama 8 bulan.
3. Setiap bulan memiliki persentase laba berbeda:
Bulan 1–2: 0%
Bulan 3–4: 10%
Bulan 5–7: 50%
Bulan 8: 20%
4. Laba tiap bulan dijumlahkan ke dalam total.
5. Program menampilkan laba setiap bulan dan total akhir.

Contoh Output:
laba bulan ke-1 sebesar: 0
laba bulan ke-2 sebesar: 0
laba bulan ke-3 sebesar: 10000000.0
laba bulan ke-4 sebesar: 10000000.0
laba bulan ke-5 sebesar: 50000000.0
laba bulan ke-6 sebesar: 50000000.0
laba bulan ke-7 sebesar: 50000000.0
laba bulan ke-8 sebesar: 20000000.0
Total laba adalah: 190000000.0

---

Latihan 3 – Simulasi Mesin ATM
Kode Program (latihan3.py)
saldo = 1000000  # saldo awal
while True:
    print(f"\nSaldo saat ini: Rp {saldo}")
    print("1. Tarik Uang")
    print("2. Keluar")
    pilihan = input("Pilih menu (1/2): ")
    if pilihan == "1":
        tarik = int(input("Masukkan jumlah penarikan: "))
        if tarik > saldo:
            print("Saldo tidak cukup!")
        elif tarik <= 0:
            print("Jumlah penarikan tidak valid!")
        else:
            saldo -= tarik
            print("Penarikan berhasil!")
    elif pilihan == "2":
        print("Terima kasih telah menggunakan ATM!")
        break
    else:
        print("Pilihan tidak valid, silakan coba lagi.")

Alur Algoritma:
1. Saldo awal diatur sebesar Rp 1.000.000.
2. Program menampilkan menu:
   1. Tarik uang
   2. Keluar
3. Jika pengguna memilih 1:
Input jumlah penarikan.
Cek apakah saldo mencukupi.
Jika cukup, saldo dikurangi dan ditampilkan pesan berhasil.
4. Jika pengguna memilih 2:
Program berhenti dengan pesan “Terima kasih telah menggunakan ATM!”.
5. Program terus berjalan hingga pengguna memilih keluar.

Contoh Output:
Saldo saat ini: Rp 1000000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 1
Masukkan jumlah penarikan: 500000
Penarikan berhasil!
Saldo saat ini: Rp 500000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 2
Terima kasih telah menggunakan ATM!

---

Langkah Menjalankan Program
1. Buka folder labpy03 di terminal.
2. Jalankan masing-masing file:
python3 latihan1.py
python3 latihan2.py
python3 latihan3.py
3. Lihat hasil sesuai dengan contoh output di atas.

---

Hasil Screenshot

📸 Screenshot latihan1.py
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/9e26d19d-a0e5-4b27-9ddc-2f37838f58df" />

📸 Screenshot latihan2.py
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/7b520b6a-c4ef-4a22-9f68-b905fb691c60" />

📸 Screenshot latihan3.py
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/bb5151b6-4c20-4b1f-9c54-c0e029e4aecd" />

---

Kesimpulan
Dari tiga latihan ini, kita belajar:
Cara menggunakan fungsi random() dan perulangan while.
Cara menghitung laba dengan logika kondisi if dan for.
Cara membuat simulasi interaktif menggunakan input() dan while.

---
