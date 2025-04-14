# 📚Program Perkalian Matriks 5x5 Python

Program ini melakukan perkalian antara dua matriks 5x5 menggunakan perulangan for untuk menghitung hasil perkalian setiap elemen, tanpa bergantung pada library eksternal.

---
## 🎯 Matriks Input
### Matriks A :
```
    [1,2,3,4,5],
    [6,7,8,9,10],
    [11,12,13,14,15],
    [16,17,18,19,20],
    [21,22,23,24,25]
```

### Matriks B :
```
    [2,4,6,8,10],
    [1,3,5,7,9],
    [2,4,6,1,2],
    [3,2,1,4,6],
    [2,1,3,4,2]
```
---
## ⚙️ Cara Perhitungan Matriks 
### Inisialisasi Hasil Matriks
```
hasil = []
```
##### Penjelasan : 
- `hasil` adalah variabel yang akan menampung matriks hasil perkalian antara Matriks A dan Matriks B.
---
### Proses Perhitungan Matriks A dan B
```
hasil = []  # Matriks kosong untuk menyimpan hasil perkalian

for i in range(5):  # Melalui setiap baris pada Matriks A
    baris = []
    for j in range(5):  # Melalui setiap kolom pada Matriks B
        total = 0
        for k in range(5):  # Perkalian elemen pada baris A dan kolom B
            total += A[i][k] * B[k][j]
        baris.append(total)
    hasil.append(baris)
```
##### Penjelasan : 
- Loop pertama (i) mengakses baris-baris pada Matriks A.
- Loop kedua (j) mengakses kolom-kolom pada Matriks B
- Loop ketiga (k) melakukan perkalian elemen baris A dengan elemen kolom B, lalu menjumlahkan hasilnya untuk menghasilkan elemen pada matriks hasil.
---
## Menampilkan hasil perkalian matriks
```
print ("Hasil perkalian matriks A dan B adalah : ")
for row in hasil : 
    print(row)
```
##### Penjelasan : 
- Setiap baris dari matriks hasil diprint satu per satu.
---
## Contoh Perhitungan Manual
Baris pertama Matriks A: ` [1, 2, 3, 4, 5] `
Kolom pertama Matriks B: ` [2, 1, 2, 3, 2] `
```
= 1×2 + 2×1 + 3×2 + 4×3 + 5×2
= 2 + 2 + 6 + 12 + 10
= 32
```
---
## Hasil dari perkalian Matriks 
Setelah perkalian dilakukan, berikut adalah hasil dari matriks A dikali matriks B:
```
[32, 35, 53, 61, 68]
[82, 105, 158, 181, 213]
[132, 175, 263, 301, 358]
[182, 245, 368, 421, 503]
[232, 315, 473, 541, 648]
```
---

### 📝Catatan
- Program ini tanpa library eksternal dan sepenuhnya menggunakan perulangan untuk perkalian matriks.
- Operasi perkalian dilakukan menggunakan nested loops untuk menghitung setiap elemen hasil dari perkalian baris A dan kolom B.
- Hasil dari setiap perkalian elemen disimpan dalam baris menggunakan metode append(), yang kemudian ditambahkan ke matriks hasil dengan append() juga.

> Amelia Nurpuspita Dewi
> Informatika - Universitas Sultan Ageng Tirtayasa

**Thank You!!**
---

