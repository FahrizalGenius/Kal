---
title: INVERS_MATRIK

---

# INVERS MATRIK 
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

Menggunakan metode ekspansi kofaktor:

$$
|A|=1 \times\left|\begin{array}{ll}
1 & 4 \\
0 & 1
\end{array}\right|
$$

Karena:

$$
\left|\begin{array}{ll}
1 & 4 \\
0 & 1
\end{array}\right|=(1 \times 1)-(4 \times 0)=1
$$

Maka:

$$
|A|=1 \times 1=1
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

Kita kalikan $A^{-1}$ dengan $B$ : 

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
- Matriks $\boldsymbol{A}$ yang kita gunakan adalah:
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

- Perkalian $A^{-1} B$ menghasilkan $(1,0,0)$, yang sesuai dengan keinginan.