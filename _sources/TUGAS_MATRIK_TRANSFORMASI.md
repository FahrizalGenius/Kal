---
title: TUGAS MATRIK TRANSFORMASI

---

# TUGAS MATRIK TRANSFORMASI
## Tugas 1

buktikan bahwa T(v1,v2)-(v1+v2,v1) andalah transformasi linier

### Langkah 1: Pahami Definisi Transformasi Linier
Sebuah transformasi 

$T: \mathbb{R}^n \rightarrow \mathbb{R}^m$ 

dikatakan linier jika memenuhi dua syarat:

 1. Aditivitas (Sifat Penjumlahan):

$T(\mathbf{u}+\mathbf{v})=T(\mathbf{u})+T(\mathbf{v})$ 

untuk semua vektor 

$\mathbf{u}, \mathbf{v}$.


2. Homogenitas (Sifat Perkalian Skalar): $T(c \mathbf{v})=c T(\mathbf{v})$

untuk semua skalar  $c$ dan vektor $\mathbf{v}$.

### Langkah 2: Verifikasi Aditivitas
Misalkan:

- $\mathbf{u}=\left(u_1, u_2\right)$

- $\mathbf{v}=\left(v_1, v_2\right)$

Langkah Perhitungan:

1. Hitung $T(\mathbf{u}+\mathbf{v})$ : 

$$
\begin{aligned}
T(\mathbf{u}+\mathbf{v}) & =T\left(u_1+v_1, u_2+v_2\right) \\
& =\left(\left(u_1+v_1\right)+\left(u_2+v_2\right), u_1+v_1\right) \\
& =\left(u_1+u_2+v_1+v_2, u_1+v_1\right)
\end{aligned}
$$

2. Hitung $T(\mathbf{u})+T(\mathbf{v})$ : 

$$
\begin{aligned}
T(\mathbf{u})+T(\mathbf{v}) & =\left(u_1+u_2, u_1\right)+\left(v_1+v_2, v_1\right) \\
& =\left(u_1+u_2+v_1+v_2, u_1+v_1\right)
\end{aligned}
$$

3. Bandingkan Hasil:

Kedua hasil di atas identik, sehingga:

$$
T(\mathbf{u}+\mathbf{v})=T(\mathbf{u})+T(\mathbf{v})
$$

Aditivitas terbukti!

### Langkah 3: Verifikasi Homogenitas

Misalkan:

- Skalar 

$c \in \mathbb{R}$

- Vektor 

$\mathbf{v}=\left(v_1, v_2\right)$

Langkah Perhitungan:
1. Hitung 

$T(c \mathbf{v})$  : 

$$
\begin{aligned}
T(c \mathbf{v}) & =T\left(c v_1, c v_2\right) \\
& =\left(c v_1+c v_2, c v_1\right) \\
& =c\left(v_1+v_2, v_1\right)
\end{aligned}
$$

2. Hitung 

$c T(\mathbf{v})$  : 

$$
c T(\mathbf{v})=c\left(v_1+v_2, v_1\right)
$$

3. Bandingkan Hasil:

Kedua hasil di atas identik, sehingga: 

$$
T(c \mathbf{v})=c T(\mathbf{v})
$$

Homogenitas terbukti!

### Langkah 4: Representasi Matriks (Konfirmasi Tambahan)

Transformasi linier dapat direpresentasikan sebagai perkalian matriks. Untuk 

$T\left(v_1, v_2\right)=\left(v_1+v_2, v_1\right)$, 

matriksnya adalah: 

$$
A=\left[\begin{array}{ll}
1 & 1 \\
1 & 0
\end{array}\right]
$$

Bukti: 

$$
\left[\begin{array}{ll}
1 & 1 \\
1 & 0
\end{array}\right]\left[\begin{array}{l}
v_1 \\
v_2
\end{array}\right]=\left[\begin{array}{c}
v_1+v_2 \\
v_1
\end{array}\right]=T\left(v_1, v_2\right) .
$$

Representasi matriks ini mengonfirmasi kelinieran $T$.

### Langkah 5: Simpulkan

Karena $T$ memenuhi kedua sifat aditivitas dan homogenitas, serta memiliki representasi matriks, maka:

$$
T \text { adalah transformasi linier. }
$$

## Tugas 2

### 1. Refleksi Terhadap Sumbu-X

Matriks: 

$$
M_x=\left[\begin{array}{cc}
1 & 0 \\
0 & -1
\end{array}\right]
$$

Langkah GeoGebra:

1. Buat titik asal:
- Ketik A $=(2,3)$ di Input Bar.

- Ketik B $=(1,-2)$ di Input Bar.

2. Buat matriks refleksi sumbu-X: 

- Ketik $M_{-} \mathrm{x}=\{\{1,0\},\{0,-1\}\}$ di Input Bar. 

3. Hitung hasil refleksi:

- Ketik A_refleksi $=$ M_x * A $\rightarrow$ Hasil: $(2,-3)$.

- Ketik B_refleksi = M_x * B $\rightarrow$ Hasil: $(1,2)$.

4. Verifikasi:

- Plot titik asli dan hasil refleksi. Pastikan titik refleksi berada di bawah sumbu-X.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/w5g63hmg?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 2. Refleksi Terhadap Sumbu-Y

Matriks: 

$$
M_y=\left[\begin{array}{cc}
-1 & 0 \\
0 & 1
\end{array}\right]
$$

Langkah GeoGebra:

1. Buat matriks refleksi sumbu-Y: 

- Ketik M_y = \{\{-1, 0\}, \{0, 1\}\} di Input Bar.

2. Hitung hasil refleksi: 

- Ketik A_refleksi $=$ M_y * A $\rightarrow$ Hasil: $(-2,3)$.

- Ketik B_refleksi $=$ M_y * B $\rightarrow$ Hasil: $(-1,-2)$. 

3. Verifikasi:

- Pastikan titik refleksi berada di sisi kiri sumbu-Y.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/dgj3rybg?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 3. Refleksi Terhadap Garis ${y}={x}$

Matriks:

$$
M_{y=x}=\left[\begin{array}{ll}
0 & 1 \\
1 & 0
\end{array}\right]
$$

Langkah GeoGebra:

1. Buat garis $y=x$ :

- Ketik $\mathrm{y}=\mathrm{x}$ di Input Bar. 

2. Buat matriks refleksi:

- Ketik M_yx = \{\{0, 1\}, \{1, 0\}\}.

3. Hitung hasil refieksi:

- Ketik A_refleksi $=$ M_yx $* A \rightarrow \operatorname{Hasil}:(3,2)$.

- Ketik B_refleksi $=$ M_yx * B $\rightarrow$ Hasil: $(-2,1)$.

4. Verifikasi:

- Pastikan titik refleksi adalah pencerminan diagonal dari titik asli.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/hewmyqh3?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 4. Refleksi Terhadap Garis $y=-x$

Matriks:

$$
M_{y=-x}=\left[\begin{array}{cc}
0 & -1 \\
-1 & 0
\end{array}\right]
$$

Langkah GeoGebra:

1. Buat garis $y=-x$ : 

- Ketik y = -x di Input Bar.

2. Buat matriks refleksi:

- Ketik M_ynx $=\{\{0,-1\},\{-1,0\}\}$

3. Hitung hasil refleksi:
4.
- Ketik A_refleksi $=$ M_ynx * $A \rightarrow$ Hasil: $(-3,-2)$.

- Ketik B_refleksi $=$ M_ynx * B $\rightarrow$ Hasil: $(2,-1)$.

4. Verifikasi: 

- Pastikan titik refleksi berada di kuadran berlawanan dari garis $y=-x$.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/fax6bukg?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 5. Refleksi Terhadap Titik Asal (Origin)

Matriks: 

$$
M_{\text {origin }}=\left[\begin{array}{cc}
-1 & 0 \\
0 & -1
\end{array}\right]
$$

Langkah GeoGebra:
1. Buat matriks refleksi origin:

- Ketik M_origin $=\{\{-1,0\},\{0,-1\}\}$.

2. Hitung hasil refieksi:

- Ketik A_refleksi $=$ M_origin * $A \rightarrow \operatorname{Hasil}:(-2,-3)$.

- Ketik B_refleksi $=$ M_origin * B $\rightarrow \operatorname{Hasil}:(-1,2)$.

3. Verifikasi:

- Pastikan titik refleksi berlawanan arah dari titik asli terhadap origin.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/uwgnshbz?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>