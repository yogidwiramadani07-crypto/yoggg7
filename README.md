#  Tugas Matriks 5×5

---

## 1. Matriks Umum

Diberikan matriks:

```
A = | a  b  c  d  e |
    | f  g  h  i  j |
    | k  l  m  n  o |
    | p  q  r  s  t |
    | u  v  w  x  y |
```

---

## 2. Determinan

Rumus ekspansi kofaktor (baris pertama):

```
det(A) = aC11 + bC12 + cC13 + dC14 + eC15
```

Dengan:

```
Cij = (-1)^(i+j) × Mij
```

Keterangan:

* **Cij** = kofaktor
* **Mij** = minor (determinan matriks 4×4)

---

## 3. Adjoint

Adjoint adalah transpose dari matriks kofaktor:

```
adj(A) = (Cij)^T
```

Langkah:

1. Hitung minor (Mij)
2. Hitung kofaktor (Cij)
3. Susun matriks kofaktor
4. Transpose

---

## 4. Invers Matriks

```
A⁻¹ = (1 / det(A)) × adj(A)
```

Syarat:

```
det(A) ≠ 0
```

---

## 5. Contoh Matriks

```
A = | 1  2  0  0  0 |
    | 0  1  3  0  0 |
    | 0  0  1  4  0 |
    | 0  0  0  1  5 |
    | 0  0  0  0  1 |
```

---

## 6. Penyelesaian

###  Determinan

Karena matriks segitiga atas:

```
det(A) = 1 × 1 × 1 × 1 × 1 = 1
```

---

###  Invers Matriks

Karena:

```
A⁻¹ = (1 / det(A)) × adj(A)
A⁻¹ = adj(A)
```

Maka:

```
A⁻¹ = | 1  -2   6   -24   120 |
       | 0   1  -3    12   -60 |
       | 0   0   1    -4    20 |
       | 0   0   0     1    -5 |
       | 0   0   0     0     1 |
```

---

###  Verifikasi

```
A × A⁻¹ = I
```

Dengan:

```
I = | 1 0 0 0 0 |
    | 0 1 0 0 0 |
    | 0 0 1 0 0 |
    | 0 0 0 1 0 |
    | 0 0 0 0 1 |
```

---

## 7. Kesimpulan

* Determinan = 1 → matriks memiliki invers
* Invers dihitung dengan:

  ```
  A⁻¹ = (1/det(A)) × adj(A)
  ```
* Matriks segitiga mempermudah perhitungan

---

## Pengurangan Matriks

### Pengertian
Pengurangan matriks dilakukan dengan mengurangkan elemen-elemen yang bersesuaian dari dua matriks yang memiliki ordo yang sama.

### Syarat
- Kedua matriks harus memiliki ukuran yang sama.

### Rumus
A − B = [aᵢⱼ − bᵢⱼ]

### Contoh

A = [5  7]  
  [8  4]

B = [2  3]  
  [1  6]

Maka,

A − B = [5−2  7−3]  
    [8−1  4−6]

= [3  4]  
 [7 -2]

---

## Pembagian Matriks

### Pengertian
Pembagian matriks dilakukan dengan mengalikan matriks pertama dengan invers dari matriks kedua.

### Rumus
A ÷ B = A × B⁻¹

### Syarat
- Matriks pembagi harus memiliki invers.
- Determinan matriks pembagi tidak sama dengan nol.

### Contoh

A = [4  2]  
  [6  8]

B = [1  2]  
  [3  4]

Maka,

A ÷ B = A × B⁻¹

---

## Penjumlahan Matriks

### Pengertian
Penjumlahan matriks dilakukan dengan menjumlahkan elemen-elemen yang bersesuaian dari dua matriks yang memiliki ordo sama.

### Syarat
- Kedua matriks harus memiliki ukuran yang sama.

### Rumus
A + B = [aᵢⱼ + bᵢⱼ]

### Contoh

A = [2  5]  
  [7  1]

B = [3  4]  
  [6  8]

Maka,

A + B = [2+3  5+4]  
    [7+6  1+8]

= [5  9]  
 [13  9]

---

# Kesimpulan

| Operasi | Syarat | Cara Perhitungan |
|----------|---------|-----------------|
| Penjumlahan Matriks | Ordo sama | Menjumlahkan elemen yang bersesuaian |
| Pengurangan Matriks | Ordo sama | Mengurangkan elemen yang bersesuaian |
| Pembagian Matriks | Matriks pembagi memiliki invers | Mengalikan dengan invers matriks pembagi |

## Catatan
- Penjumlahan dan pengurangan hanya dapat dilakukan pada matriks yang berordo sama.
- Pembagian matriks dilakukan melalui invers matriks.
- Tidak semua matriks memiliki invers.

## 8. Catatan

Perhitungan matriks 5×5 secara manual cukup panjang, sehingga biasanya digunakan bantuan software seperti Python atau MATLAB. Namun, pemahaman konsep tetap penting.
