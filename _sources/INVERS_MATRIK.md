---
title: INVERS MATRIK

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

### Buat Persamaan 3x3    

$$
\left\{\begin{array}{l}
2 x-y+0 z=2 \\
x+3 y-z=1 \\
0 x+2 y+4 z=0
\end{array}\right.
$$

Dari sistem ini, kita bisa tulis dalam bentuk matriks sebagai:


$$
A=\left[\begin{array}{ccc}
2 & -1 & 0 \\
1 & 3 & -1 \\
0 & 2 & 4
\end{array}\right]
$$


dan


$$
B=\left[\begin{array}{l}
2 \\
1 \\
0
\end{array}\right]
$$


Kita ingin mencari invers $A^{-1}$ dan menunjukkan bahwa:


$$
A^{-1} \times B=\left[\begin{array}{l}
1 \\
0 \\
0
\end{array}\right]
$$


Sehingga solusinya adalah 

$x=1, y=0, z=0$.

### Langkah 2: Bentuk Augmented Matrix   $[A \mid I]$
Kita gabungkan $A$ dengan matriks identitas $I$ : 


$$
[A \mid I]=\left[\begin{array}{ccc|ccc}
2 & -1 & 0 & \mid 1 & 0 & 0 \\
1 & 3 & -1 & \mid 0 & 1 & 0 \\
0 & 2 & 4 & 0 & 0 & 1
\end{array}\right]
$$


### Langkah 3: Buat Elemen (1,1) Menjadi 1
Saat ini, elemen pertama (1,1) adalah 2. Kita ubah menjadi 1 dengan membagi baris pertama dengan 2:


$$
\begin{gathered}
R_1 \leftarrow \frac{1}{2} R_1 \\
{\left[\begin{array}{ccc|ccc}
1 & -\frac{1}{2} & 0 & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
1 & 3 & -1 & 0 & 1 & 0 \\
0 & 2 & 4 & 0 & 0 & 1
\end{array}\right]}
\end{gathered}
$$

### Langkah 4: Nol-kan Elemen di Bawah (1,1)
Kita nol-kan elemen $(2,1)$ menggunakan operasi baris:


$$
\begin{gathered}
R_2 \leftarrow R_2-R_1 \\
{\left[\begin{array}{cccccc}
1 & -\frac{1}{2} & 0 & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
0 & \frac{7}{2} & -1 & -\frac{1}{2} & 1 & 0 \\
0 & 2 & 4 & \mid 0 & 0 & 1
\end{array}\right]}
\end{gathered}
$$

### Langkah 5: Buat Elemen $(2,2)$ Menjadi 1
Saat ini, elemen $(2,2)$ adalah $\frac{7}{2}$. Kita ubah menjadi 1 dengan membagi baris kedua dengan $\frac{7}{2}$ : 


$$
\begin{gathered}
R_2 \leftarrow \frac{2}{7} R_2 \\
{\left[\begin{array}{cccccc}
1 & -\frac{1}{2} & 0 & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
0 & 1 & -\frac{2}{7} & \left\lvert\,-\frac{1}{7}\right. & \frac{2}{7} & 0 \\
0 & 2 & 4 & \mid 0 & 0 & 1
\end{array}\right]}
\end{gathered}
$$

### Langkah 6: Nol-kan Elemen di Bawah (2,2)

Kita nol-kan elemen (3,2):


$$
\begin{gathered}
R_3 \leftarrow R_3-2 R_2 \\
{\left[\begin{array}{cccccc}
1 & -\frac{1}{2} & 0 & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
0 & 1 & -\frac{2}{7} & \left\lvert\,-\frac{1}{7}\right. & \frac{2}{7} & 0 \\
0 & 0 & \frac{30}{7} & \left\lvert\, \frac{2}{7}\right. & -\frac{4}{7} & 1
\end{array}\right]}
\end{gathered}
$$

### Langkah 7: Buat Elemen (3,3) Menjadi 1
Saat ini, elemen $(3,3)$ adalah $\frac{30}{7}$. Kita ubah menjadi 1 dengan membagi baris ketiga dengan $\frac{30}{7}$ : 


$$
\begin{gathered}
R_3 \leftarrow \frac{7}{30} R_3 \\
{\left[\begin{array}{cccccc}
1 & -\frac{1}{2} & 0 & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\
0 & 1 & -\frac{2}{7} & -\frac{1}{7} & \frac{2}{7} & 0 \\
0 & 0 & 1 & \left\lvert\, \frac{1}{15}\right. & -\frac{2}{15} & \frac{7}{30}
\end{array}\right]}
\end{gathered}
$$

### Langkah 8: Nol-kan Elemen di Atas (3,3)
Kita nol-kan elemen $(1,2)$ dan $(2,3)$.
- Untuk baris (1,2):


$$
R_1 \leftarrow R_1+\frac{1}{2} R_2
$$


- Untuk baris (2,3):


$$
R_2 \leftarrow R_2+\frac{2}{7} R_3
$$

- Untuk baris (1,3)

$$
R_1 \leftarrow R_1 + \frac{1}{7} R_3
$$

Hasil akhirnya: 


$$
\left[\begin{array}{cccccc}
1 & 0 & 0 & \left\lvert\, \frac{8}{15}\right. & -\frac{1}{5} & \frac{7}{20} \\
0 & 1 & 0 & \left\lvert\,-\frac{1}{5}\right. & \frac{3}{5} & -\frac{7}{10} \\
0 & 0 & 1 & \left\lvert\, \frac{1}{15}\right. & -\frac{2}{15} & \frac{7}{30}
\end{array}\right]
$$


Maka inversnya adalah: 


$$
A^{-1}=\left[\begin{array}{ccc}
\frac{8}{15} & -\frac{1}{5} & \frac{7}{20} \\
-\frac{1}{5} & \frac{3}{5} & -\frac{7}{10} \\
\frac{1}{15} & -\frac{2}{15} & \frac{7}{30}
\end{array}\right]
$$

### Langkah 9: Hitung $A^{-1} \times B$
Dengan $B=\left[\begin{array}{l}2 \\ 1 \\ 0\end{array}\right]$  , kita hitung: 


$$
A^{-1} \times B=\left[\begin{array}{ccc}
\frac{8}{15} & -\frac{1}{5} & \frac{7}{20} \\
-\frac{1}{5} & \frac{3}{5} & -\frac{7}{10} \\
\frac{1}{15} & -\frac{2}{15} & \frac{7}{30}
\end{array}\right] \times\left[\begin{array}{l}
2 \\
1 \\
0
\end{array}\right]
$$

Hasilnya:


$$
\left[\begin{array}{c}
\left(\frac{8}{15} \times 2\right)+\left(-\frac{1}{5} \times 1\right)+\left(\frac{7}{20} \times 0\right) \\
\left(-\frac{1}{5} \times 2\right)+\left(\frac{3}{5} \times 1\right)+\left(-\frac{7}{10} \times 0\right) \\
\left(\frac{1}{15} \times 2\right)+\left(-\frac{2}{15} \times 1{ }^{\prime}+\left(\frac{7}{30} \times 0\right)\right.
\end{array}\right]=\left[\begin{array}{l}
1 \\
0 \\
0
\end{array}\right]
$$