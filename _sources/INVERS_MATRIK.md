---
title: INVERS_MATRIK

---

# INVERS MATRIK 
### Definisi Matriks Invers

Matriks invers adalah matriks yang jika dikalikan dengan matriks aslinya menghasilkan matriks identitas.

Secara matematis, jika ${A}$ adalah sebuah matriks persegi, maka inversnya, yang ditulis sebagai $A^{-1}$, memenuhi persamaan:

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
2x+3 y- z=5 \\
x-2y+4 z=-3 \\
3 x+y+2z=7
\end{array}\right.
$$

### 1. Diketahui Matriks ${A}$

Kita memiliki matriks $A$ : 

$$
A=\left[\begin{array}{ccc}
2 & 3 & -1 \\
1 & -2 & 4 \\
3 & 1 & 2
\end{array}\right]
$$

Untuk mencari invers $\left(A^{-1}\right)$, kita buat matriks augmented dengan identitas: 

$$
[A \mid I]=\left[\begin{array}{cccccc}
2 & 3 & -1 & \mid 1 & 0 & 0 \\
1 & -2 & 4 & \mid 0 & 1 & 0 \\
3 & 1 & 2 & \mid 0 & 0 & 1
\end{array}\right]
$$

Tujuan: Kita harus mengubah bagian kiri menjadi identitas $I$, dan bagian kanan akan menjadi invers $A^{-1}$.

### 2. Membuat Elemen $(1,1)$ Menjadi 1

Saat ini, elemen pertama $(1,1)$ adalah 2, jadi kita bagi seluruh baris 1 dengan 2:

$$
\begin{gathered}
R_1 \rightarrow \frac{1}{2} R_1 \\
{\left[\begin{array}{ccc|ccc}
1 & \frac{3}{2} & -\frac{1}{2} & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
1 & -2 & 4 & 0 & 1 & 0 \\
3 & 1 & 2 & 0 & 0 & 1
\end{array}\right]}
\end{gathered}
$$

### 3. Menghilangkan Elemen Kolom 1 di Baris 2 dan 3

Kita buat elemen $(2,1)$ dan $(3,1)$ menjadi 0.

- Baris $2 \rightarrow R_2=R_2-R_1$
- Baris $3 \rightarrow R_3=R_3-3 R_1$


#### Langkah 1: Menjadikan Elemen (2,1) = 0
Elemen ( 2,1 ) saat ini adalah 1.
Untuk mengubahnya menjadi 0, kita lakukan operasi baris:

$$
R_2=R_2-R_1
$$

Perhitungan Baris 2 Baru ( $\mathbf{R}_{\mathbf{2}}$ )
Setiap elemen baris 2 dikurangi baris 1.


\begin{array}{|c|c|c|c|}
\hline
\text{Elemen} & R_2 \text{ Lama} & R_1 & R_2 - R_1 \text{ (Baris 2 Baru)} \\
\hline
(2,1) & 1 & 1 & 1 - 1 = 0 \\
\hline
(2,2) & -2 & \frac{3}{2} & -2 - \frac{3}{2} = -\frac{4}{2} - \frac{3}{2} = -\frac{7}{2} \\
\hline
(2,3) & 4 & -\frac{1}{2} & 4 - (-\frac{1}{2}) = 4 + \frac{1}{2} = \frac{8}{2} + \frac{1}{2} = \frac{9}{2} \\
\hline
(2,4) & 0 & \frac{1}{2} & 0 - \frac{1}{2} = -\frac{1}{2} \\
\hline
(2,5) & 1 & 0 & 1 - 0 = 1 \\
\hline
(2,6) & 0 & 0 & 0 - 0 = 0 \\
\hline
\end{array}


Hasil baris 2 baru:
$$
\left(0,-\frac{7}{2}, \frac{9}{2}, \left\lvert\,-\frac{1}{2}\right., 1,0\right)
$$

#### Langkah 2: Menjadikan Elemen (3,1) = 0
Elemen ( 3,1 ) saat ini adalah 3.
Untuk mengubahnya menjadi 0, kita lakukan operasi baris:

$$
R_3=R_3-3 R_1
$$

Perhitungan Baris 3 Baru ( $\mathbf{R}_3$ )
Setiap elemen baris $\mathbf{3}$ dikurangi $\mathbf{3 \times}$ baris 1 .

\begin{array}{|c|c|c|c|}
\hline
\text{Elemen} & R_3 \text{ Lama} & 3 \times R_1 & R_3 - 3R_1 \text{ (Baris 3 Baru)} \\
\hline
(3,1) & 3 & 3 \times 1 = 3 & 3 - 3 = 0 \\
\hline
(3,2) & 1 & 3 \times \frac{3}{2} = \frac{9}{2} & 1 - \frac{9}{2} = \frac{2}{2} - \frac{9}{2} = -\frac{7}{2} \\
\hline
(3,3) & 2 & 3 \times (-\frac{1}{2}) = -\frac{3}{2} & 2 - (-\frac{3}{2}) = 2 + \frac{3}{2} = \frac{4}{2} + \frac{3}{2} = \frac{11}{2} \\
\hline
(3,4) & 0 & 3 \times \frac{1}{2} = \frac{3}{2} & 0 - \frac{3}{2} = -\frac{3}{2} \\
\hline
(3,5) & 0 & 3 \times 0 = 0 & 0 - 0 = 0 \\
\hline
(3,6) & 1 & 3 \times 0 = 0 & 1 - 0 = 1 \\
\hline
\end{array}

Hasil baris 3 baru:
$$
\left(0,-\frac{7}{2}, \frac{11}{2}, \left\lvert\,-\frac{3}{2}\right., 0,1\right)
$$

#### Hasil matriks setelah eliminasi:

$$
\left[\begin{array}{cccccc}
1 & \frac{3}{2} & -\frac{1}{2} & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
0 & -\frac{7}{2} & \frac{9}{2} & \left\lvert\,-\frac{1}{2}\right. & 1 & 0 \\
0 & -\frac{7}{2} & \frac{11}{2} & -\frac{3}{2} & 0 & 1
\end{array}\right]
$$

### 4. Membuat Elemen $(2,2)$ Menjadi 1

Saat ini, elemen $(2,2)$ adalah $-\frac{7}{2}$. Untuk menjadikannya 1 , kita bagi baris 2 dengan $-\frac{7}{2}$ : 

$$
R_2 \rightarrow \frac{2}{-7} R_2
$$

Perhitungan Baris 2 Baru

Kita lakukan pembagian untuk setiap elemen di baris 2:


\begin{array}{|c|c|c|c|}
\hline
\text{Elemen} & \text{Nilai Lama } R_2 & \text{Dibagi } -\frac{7}{2} & \text{Hasil Baru } R_2 \\
\hline
(2,1) & 0 & 0 \div\left(-\frac{7}{2}\right) & 0 \\
\hline
(2,2) & -\frac{7}{2} & \left(-\frac{7}{2}\right) \div\left(-\frac{7}{2}\right) & 1 \\
\hline
(2,3) & \frac{9}{2} & \left(\frac{9}{2}\right) \div\left(-\frac{7}{2}\right) & -\frac{9}{7} \\
\hline
(2,4) & -\frac{1}{2} & \left(-\frac{1}{2}\right) \div\left(-\frac{7}{2}\right) & \frac{1}{7} \\
\hline
(2,5) & 1 & 1 \div\left(-\frac{7}{2}\right) & -\frac{2}{7} \\
\hline
(2,6) & \mathbf{0} & 0 \div\left(-\frac{7}{2}\right) & 0 \\
\hline
\end{array}


Hasil baris 2 setelah pembagian:

$$
\left(0,1,-\frac{9}{7}, \left\lvert\, \frac{1}{7}\right.,-\frac{2}{7}, 0\right)
$$
Hasilnya:

$$
\left[\begin{array}{cccccc}
1 & \frac{3}{2} & -\frac{1}{2} & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
0 & 1 & -\frac{9}{7} & \left\lvert\, \frac{1}{7}\right. & -\frac{2}{7} & 0 \\
0 & -\frac{7}{2} & \frac{11}{2} & \left\lvert\,-\frac{3}{2}\right. & 0 & 1
\end{array}\right]
$$

### 5. Menghilangkan Elemen Kolom 2 di Baris 1 dan 3
- Baris $1 \rightarrow R_1=R_1-\frac{3}{2} R_2$
- Baris $3 \rightarrow R_3=R_3+\frac{7}{2} R_2$



#### Perhitungan Baris 1 Baru

Setiap elemen di baris 1 dikurangi $\frac{3}{2} \times$ baris 2 .

\begin{array}{|c|c|c|c|}
\hline
\text{Elemen} & \text{Nilai Lama } R_1 & \frac{3}{2} \times R_2 & R_1 - \frac{3}{2} R_2 \text{ (Baris 1 Baru)} \\
\hline
(1,1) & 1 & \frac{3}{2} \times 0 = 0 & 1 - 0 = 1 \\
\hline
(1,2) & \frac{3}{2} & \frac{3}{2} \times 1 = \frac{3}{2} & \frac{3}{2} - \frac{3}{2} = 0 \\
\hline
(1,3) & -\frac{1}{2} & \frac{3}{2} \times \left(-\frac{9}{7}\right) = -\frac{27}{14} & -\frac{1}{2} - \left(-\frac{27}{14}\right) = -\frac{7}{14} + \frac{27}{14} = \frac{20}{14} = \frac{10}{7} \\
\hline
(1,4) & \frac{1}{2} & \frac{3}{2} \times \frac{1}{7} = \frac{3}{14} & \frac{1}{2} - \frac{3}{14} = \frac{7}{14} - \frac{3}{14} = \frac{4}{14} = \frac{2}{7} \\
\hline
(1,5) & 0 & \frac{3}{2} \times \left(-\frac{2}{7}\right) = -\frac{6}{14} & 0 - \left(-\frac{6}{14}\right) = \frac{6}{14} = \frac{3}{7} \\
\hline
(1,6) & 0 & \frac{3}{2} \times 0 = 0 & 0 - 0 = 0 \\
\hline
\end{array}

Hasil baris 1 baru:

$$
\left(1,0, \frac{10}{7}, \left\lvert\, \frac{2}{7}\right., \frac{3}{7}, 0\right)
$$

#### Perhitungan Baris 3 Baru

Setiap elemen di baris 3 ditambah $\frac{7}{2} \times$ baris 2 .

\begin{array}{|c|c|c|c|}
\hline
\text{Elemen} & \text{Nilai Lama } R_3 & \frac{7}{2} \times R_2 & R_3 + \frac{7}{2} R_2 \text{ (Baris 3 Baru)} \\
\hline
(3,1) & 0 & \frac{7}{2} \times 0 = 0 & 0 + 0 = 0 \\
\hline
(3,2) & -\frac{7}{2} & \frac{7}{2} \times 1 = \frac{7}{2} & -\frac{7}{2} + \frac{7}{2} = 0 \\
\hline
(3,3) & \frac{11}{2} & \frac{7}{2} \times \left(-\frac{9}{7}\right) = -\frac{63}{14} = -\frac{9}{2} & \frac{11}{2} - \frac{9}{2} = \frac{2}{2} = 1 \\
\hline
(3,4) & -\frac{3}{2} & \frac{7}{2} \times \frac{1}{7} = \frac{1}{2} & -\frac{3}{2} + \frac{1}{2} = -\frac{2}{2} = -1 \\
\hline
(3,5) & 0 & \frac{7}{2} \times \left(-\frac{2}{7}\right) = -\frac{14}{14} = -1 & 0 - 1 = -1 \\
\hline
(3,6) & 1 & \frac{7}{2} \times 0 = 0 & 1 + 0 = 1 \\
\hline
\end{array}

Hasil baris 3 baru:
$$
(0,0,1, \mid-1,-1,1)
$$

Hasil matriks:

$$
\left[\begin{array}{cccccc}
1 & 0 & \frac{10}{17} & \left\lvert\, \frac{2}{7}\right. & \frac{3}{7} & 0 \\
0 & 1 & -\frac{9}{7} & \left\lvert\, \frac{1}{7}\right. & -\frac{2}{7} & 0 \\
0 & 0 & 1 & \left\lvert\,-1\right. & -1 & 1
\end{array}\right]
$$

### 6. Mengubah Elemen (1,3) dan (2,3) menjadi 0

$$
\left[\begin{array}{cccccc}
1 & 0 & \frac{10}{17} & \left\lvert\, \frac{2}{7}\right. & \frac{3}{7} & 0 \\
0 & 1 & -\frac{9}{7} & \left\lvert\, \frac{1}{7}\right. & -\frac{2}{7} & 0 \\
0 & 0 & 1 & \left\lvert\,-1\right. & -1 & 1
\end{array}\right]
$$

Langkah 1: Menghilangkan Elemen (1,3)
Dari baris 1:
$$
R_1 \rightarrow R_1-\left(\frac{10}{17} \times R_3\right)
$$

Hitung setiap elemen baru pada baris 1:
$$
R_1=R_1-\frac{10}{17} R_3
$$

Untuk setiap elemen di baris 1:

\begin{array}{|c|c|c|}
\hline 
\textbf{Elemen Lama } R_1 & \frac{10}{17} \times R_3 & \textbf{Hasil Baru } R_1 \\
\hline
(\mathbf{1 , 1 )}: 1 & 0 & 1 \\
\hline
(\mathbf{1}, \mathbf{2}): 0 & 0 & 0 \\
\hline
(\mathbf{1}, \mathbf{3}): \frac{10}{17} & \frac{10}{17} \times 1=\frac{10}{17} & \frac{10}{17}-\frac{10}{17}=0 \\
\hline
(\mathbf{1 , 4 )}: \frac{2}{7} & \frac{10}{17} \times(-1)=-\frac{10}{17} & \frac{2}{7}-\frac{10}{17} \\
\hline
(\mathbf{1}, \mathbf{5}): \frac{3}{7} & \frac{10}{17} \times(-1)=-\frac{10}{17} & \frac{3}{7}-\frac{10}{17} \\
\hline
(\mathbf{1}, \mathbf{6}): 0 & \frac{10}{17} \times 1=\frac{10}{17} & 0-\frac{10}{17}=-\frac{10}{17} \\
\hline
\end{array}

Menyederhanakan elemen $(1,4)$ dan $(1,5):$
$$
\begin{aligned}
& \frac{2}{7}-\frac{10}{17}=\frac{34}{119}-\frac{70}{119}=-\frac{36}{119} \\
& \frac{3}{7}-\frac{10}{17}=\frac{51}{119}-\frac{70}{119}=-\frac{19}{119}
\end{aligned}
$$

Sehingga, baris 1 yang baru adalah:
$$
\left[\begin{array}{lll|lll}
1 & 0 & 0 & -\frac{36}{119} & -\frac{19}{119} & -\frac{10}{17}
\end{array}\right]
$$

Langkah 2: Menghilangkan Elemen (2,3)
Dari baris 2:
$$
R_2 \rightarrow R_2+\left(\frac{9}{7} \times R_3\right)
$$

Hitung setiap elemen baru pada baris 2:
$$
R_2=R_2+\frac{9}{7} R_3
$$

Untuk setiap elemen di baris 2:

\begin{array}{|c|c|c|}
\hline 
\textbf{Elemen Lama } R_2 & \frac{9}{7} \times R_3 & \textbf{Hasil Baru } R_2 \\
\hline
(2,1): 0 & 0 & 0 \\
\hline
(2,2): 1 & 0 & 1 \\
\hline
(2,3): -\frac{9}{7} & \frac{9}{7} \times 1 = \frac{9}{7} & -\frac{9}{7}+\frac{9}{7} = 0 \\
\hline
(2,4): \frac{1}{7} & \frac{9}{7} \times (-1) = -\frac{9}{7} & \frac{1}{7} - \frac{9}{7} = -\frac{8}{7} \\
\hline
(2,5): -\frac{2}{7} & \frac{9}{7} \times (-1) = -\frac{9}{7} & -\frac{2}{7} - \frac{9}{7} = -\frac{11}{7} \\
\hline
(2,6): 0 & \frac{9}{7} \times 1 = \frac{9}{7} & 0 + \frac{9}{7} = \frac{9}{7} \\
\hline
\end{array}

Sehingga, baris 2 yang baru adalah:
$$
\left[\begin{array}{lll|lll}
0 & 1 & 0 & -\frac{8}{7} & -\frac{11}{7} & \frac{9}{7}
\end{array}\right]
$$

Hasil Akhir Setelah Transformasi
Setelah menghilangkan elemen $(1,3)$ dan $(2,3)$, matriks menjadi:
$$
\left[\begin{array}{cccccc}
1 & 0 & 0 & \left\lvert\,-\frac{36}{119}\right. & -\frac{19}{119} & -\frac{10}{17} \\
0 & 1 & 0 & -\frac{8}{7} & -\frac{11}{7} & \frac{9}{7} \\
0 & 0 & 1 & -1 & -1 & 1
\end{array}\right]
$$