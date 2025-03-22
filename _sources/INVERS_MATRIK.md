---
title: INVERS_MATRIK

---

# INVERS MATRIK 
### Definisi Matriks Invers

Matriks invers adalah matriks yang jika dikalikan dengan matriks aslinya menghasilkan matriks identitas.

Secara matematis, jika $\boldsymbol{A}$ adalah sebuah matriks persegi, maka inversnya, yang ditulis sebagai $A^{-1}$, memenuhi persamaan:

$$
A \times A^{-1}=A^{-1} \times A=I
$$

di mana $I$ adalah matriks identitas, yaitu matriks dengan angka 1 di diagonal utama dan $\mathbf{0}$ di tempat lainnya.
Contoh matriks identitas untuk ukuran $2 \times 2$ : 

$$
I=\left[\begin{array}{ll}
1 & 0 \\
0 & 1
\end{array}\right]
$$

dan untuk ukuran $3 \times 3$ : 

$$
I=\left[\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right]
$$
### Syarat Suatu Matriks Memiliki Invers

Tidak semua matriks memiliki invers. Suatu matriks $A$ bisa memiliki invers $A^{-1}$ jika memenuhi dua syarat berikut:
1. Matriks harus berbentuk persegi $\rightarrow$ jumlah baris harus sama dengan jumlah kolom.
2. Determinan tidak boleh nol $\rightarrow|A| \neq 0$.

Jika determinannya nol $(|A|=0)$, maka matriks disebut singular dan tidak memiliki invers.

## MATRIK 3 PERSAMAAN

$$
\left\{\begin{array}{l}
x+2 y+3 z=1 \\
0 x+y+4 z=0 \\
0 x+0 y+z=0
\end{array}\right.
$$

Yang dapat dituliskan dalam bentuk matriks:

$$
A X=B
$$

Dengan:

$$
\begin{gathered}
A=\left[\begin{array}{lll}
1 & 2 & 3 \\
0 & 1 & 4 \\
0 & 0 & 1
\end{array}\right] \\
X=\left[\begin{array}{l}
x \\
y \\
z
\end{array}\right] \\
B=\left[\begin{array}{l}
1 \\
0 \\
0
\end{array}\right]
\end{gathered}
$$

Untuk mencari $X$, kita harus mencari invers dari matriks $A$, yaitu $A^{-1}$, dan mengalikannya dengan $B$ 

$$
X=A^{-1} B
$$

## Langkah-langkah mencari invers matriks ${A}$ :
### 1. Hitung Determinan $|A|$

Determinan dari matriks ${A}$ dihitung dengan rumus:

$$
|A|=\left|\begin{array}{lll}
1 & 2 & 3 \\
0 & 1 & 4 \\
0 & 0 & 1
\end{array}\right|
$$

Menggunakan metode ekspansi kofaktor pilih baris pertama untuk ekspansi:

$$
|A|=1 \times\left|\begin{array}{cc}
1 & 4 \\
0 & 1
\end{array}\right|-2 \times\left|\begin{array}{ll}
0 & 4 \\
0 & 1
\end{array}\right|+3 \times\left|\begin{array}{ll}
0 & 1 \\
0 & 0
\end{array}\right|
$$
Hasil Perhitungan
Sekarang hitunglah determinannya satu per satu:
1. Determinasi submatriks pertama:

$$
\left|\begin{array}{ll}
1 & 4 \\
0 & 1
\end{array}\right|=(1 \times 1)-(4 \times 0)=1
$$

2. Determinasi submatriks kedua:

$$
\left|\begin{array}{ll}
0 & 4 \\
0 & 1
\end{array}\right|=(0 \times 1)-(4 \times 0)=0
$$

3. Determinasi submatriks ketiga:

$$
\left|\begin{array}{ll}
0 & 1 \\
0 & 0
\end{array}\right|=(0 \times 0)-(1 \times 0)=0
$$

Sehingga:
$$
|A|=1 \times 1-2 \times 0+3 \times 0=1
$$


Karena $|{A}| \neq 0$, maka matriks memiliki invers.
### 2. Hitung Matriks Kofaktor

Matriks kofaktor diperoleh dengan mencari determinan minor untuk setiap elemen $a_{i j}$.


$$
\text { Kofaktor }(A)=\left[\begin{array}{ccc}
\left|\begin{array}{ll}
1 & 4 \\
0 & 1
\end{array}\right| & -\left|\begin{array}{ll}
0 & 4 \\
0 & 1
\end{array}\right| & \left|\begin{array}{ll}
0 & 1 \\
0 & 1
\end{array}\right| \\
-\left|\begin{array}{ll}
2 & 3 \\
0 & 1
\end{array}\right| & \left|\begin{array}{cc}
1 & 3 \\
0 & 1
\end{array}\right| & -\left|\begin{array}{rr}
1 & 2 \\
0 & 0
\end{array}\right| \\
\left|\begin{array}{ll}
2 & 3 \\
1 & 4
\end{array}\right| & -\left|\begin{array}{ll}
1 & 3 \\
0 & 4
\end{array}\right| & \left|\begin{array}{cc}
1 & 2 \\
0 & 1
\end{array}\right|
\end{array}\right]
$$

Setelah perhitungan minor, kita mendapatkan:

$$
\operatorname{Kofaktor}(A)=\left[\begin{array}{ccc}
1 & 0 & 0 \\
-2 & 1 & 0 \\
5 & -4 & 1
\end{array}\right]
$$

### 3. Transpose Matriks Kofaktor (Matriks Adjoin)

Transpose dari matriks kofaktor adalah:

$$
\operatorname{Adjoin}(A)=\left[\begin{array}{ccc}
1 & -2 & 5 \\
0 & 1 & -4 \\
0 & 0 & 1
\end{array}\right]
$$

### 4. Hitung Invers Matriks $A$

Menggunakan rumus

$$
A^{-1}=\frac{1}{|A|} \times \operatorname{Adjoin}(A)
$$

Karena $|A|=1$, maka

$$
A^{-1}=\left[\begin{array}{ccc}
1 & -2 & 5 \\
0 & 1 & -4 \\
0 & 0 & 1
\end{array}\right]
$$

5. Hitung $X=A^{-1} B$

lalu kalikan $A^{-1}$ dengan $B$ : 

$$
X=\left[\begin{array}{ccc}
1 & -2 & 5 \\
0 & 1 & -4 \\
0 & 0 & 1
\end{array}\right] \times\left[\begin{array}{l}
1 \\
0 \\
0
\end{array}\right]
$$

Perhitungan baris per baris:

- $x=(1 \times 1)+(-2 \times 0)+(5 \times 0)=1$
- $y=(0 \times 1)+(1 \times 0)+(-4 \times 0)=0$
- $z=(0 \times 1)+(0 \times 0)+(1 \times 0)=0$

Sehingga: 

$$
X=\left[\begin{array}{l}
1 \\
0 \\
0
\end{array}\right]
$$

#### Kesimpulan
- Matriks $\boldsymbol{A}$ yang digunakan adalah:
- 
$$
\left[\begin{array}{lll}
1 & 2 & 3 \\
0 & 1 & 4 \\
0 & 0 & 1
\end{array}\right]
$$

- Inversnya:

$$
\left[\begin{array}{ccc}
1 & -2 & 5 \\
0 & 1 & -4 \\
0 & 0 & 1
\end{array}\right]
$$

- Perkalian $A^{-1} B$ menghasilkan $(1,0,0)$.