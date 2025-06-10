---
title: perkalian_silang

---

# Cross dot 

Perkalian silang adalah operasi matematika pada dua vektor dalam ruang tiga dimensi yang menghasilkan vektor baru yang tegak lurus terhadap kedua vektor awal. Operasi ini disebut juga cross product dan digunakan untuk menentukan arah dan luas bidang yang dibentuk oleh kedua vektor. Hasil dari perkalian silang adalah vektor dengan arah ditentukan oleh aturan tangan kanan, dan panjangnya sama dengan luas jajar genjang yang dibentuk oleh kedua vektor tersebut. Perkalian silang hanya berlaku untuk vektor dalam tiga dimensi dan penting dalam berbagai bidang seperti fisika, teknik, dan grafik komputer.
## Menggunakan determinan Untuk perkalian silang 


### Soal
- Diketahui:

$$
\mathrm{u}=(1,1,1), \quad \mathrm{v}=(2,1,1)
$$

- Rumus Perkalian Silang:

Jika:

$$
\mathbf{u}=\left(u_1, u_2, u_3\right), \quad \mathbf{v}=\left(v_1, v_2, v_3\right)
$$

Maka:

$$
\mathbf{u} \times \mathbf{v}=\left(u_2 v_3-u_3 v_2, u_3 v_1-u_1 v_3, u_1 v_2-u_2 v_1\right)
$$

- Substitusi komponen:

Dari soal:

- $u_1=1, u_2=1, u_3=1$
- $v_1=2, v_2=1, v_3=1$

Gunakan rumus:

$$
\begin{gathered}
\mathbf{u} \times \mathbf{v}=(1 \cdot 1-1 \cdot 1,1 \cdot 2-1 \cdot 1,1 \cdot 1-1 \cdot 2) \\
=(1-1,2-1,1-2) \\
=(0,1,-1)
\end{gathered}
$$

- Hasil Akhir:

$$
\mathbf{u} \times \mathbf{v}=(0,1,-1)
$$

- Alternatif: Metode Determinan

Gunakan determinan dari matriks:

$$
u \times v=\left|\begin{array}{ccc}
i & j & k \\
1 & 1 & 1 \\
2 & 1 & 1
\end{array}\right|
$$

Hitung:

$$
\begin{gathered}
=\mathrm{i}(1 \cdot 1-1 \cdot 1)-\mathrm{j}(1 \cdot 1-1 \cdot 2)+\mathrm{k}(1 \cdot 1-1 \cdot 2) \\
=\mathrm{i}(0)-\mathrm{j}(-1)+\mathrm{k}(-1) \\
=0 \mathrm{i}+1 \mathrm{j}-1 \mathrm{k}=(0,1,-1)
\end{gathered}
$$

#### Geogebra

<iframe src="https://www.geogebra.org/classic/z7zcmumn?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>


## Definisi Hasil Kali Silang (Cross Product) Vektor
Hasil kali silang (disebut juga cross product) antara dua vektor u dan v adalah vektor baru yang:
- Tegak lurus terhadap vektor u dan v
- Arahnya ditentukan dengan aturan tangan kanan (right-hand rule)
- Panjangnya sebesar luas jajar genjang yang dibentuk oleh u dan v

## Rumus Cross Product ( $\mathbf{u} \times \mathbf{v}$ ):
Jika:

- $\mathrm{u}=\left(\mathrm{u}_1, \mathrm{u}_2, \mathrm{u}_3\right)$
- $\mathbf{v}=\left(\mathbf{v}_1, \mathbf{v}_2, \mathbf{v}_3\right)$

Maka:

$$
\mathbf{u} \times \mathbf{v}=\left(u_2 v_3-u_3 v_2, u_3 v_1-u_1 v_3, u_1 v_2-u_2 v_1\right)
$$

Contoh:
Misal:

- $\mathrm{u}=(1,2,3)$
- $v=(4,5,6)$

Maka:

$$
\begin{aligned}
& u \times v=(2 \cdot 6-3 \cdot 5,3 \cdot 4-1 \cdot 6,1 \cdot 5-2 \cdot 4) \\
& \quad=(12-15,12-6,5-8)=(-3,6,-3)
\end{aligned}
$$

## Contoh Soal:
Diketahui dua vektor.

$$
\mathbf{u}=(2,3,4), \quad \mathbf{v}=(1,5,2)
$$

Hitunglah:

$$
u \times v
$$

Langkah-langkah:

Gunakan rumus perkalian silang:

$$
\mathbf{u} \times \mathbf{v}=\left(u_2 v_3-u_3 v_2, u_3 v_1-u_1 v_3, u_1 v_2-u_2 v_1\right)
$$

Substitusi nilai-nilai:
- $u_1=2, u_2=3, u_3=4$
- $v_1=1, v_2=5, v_3=2$

## Hitung Komponen-komponennya:
1. Komponen x : 

$$
u_2 v_3-u_3 v_2=3 \cdot 2-4 \cdot 5=6-20=-14
$$

2. Komponen y: 

$$
u_3 v_1-u_1 v_3=4 \cdot 1-2 \cdot 2=4-4=0
$$

3. Komponen z:

$$
u_1 v_2-u_2 v_1=2 \cdot 5-3 \cdot 1=10-3=7
$$

## Hasil Akhir:
$$
\mathbf{u} \times \mathbf{v}=(-14,0,7)
$$


## Tugas Cross Dot
## Soal 1
1. Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u}=\left[\begin{array}{l}1 \\ 2\end{array}\right]$ dan $\vec{v}=\left[\begin{array}{l}2 \\ 1\end{array}\right]$.
2. Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u}=\left[\begin{array}{l}2 \\ 0\end{array}\right]$ dan $\vec{v}=\left[\begin{array}{l}0 \\ 3\end{array}\right]$.
3. Tentukan luas segitiga dengan titik-titik sudut $(0,0,0),(1,3,-1)$, dan $(2,1,1)$.
4. Tentukan luas segitiga dengan titik-titik sudut $(5,2,-1),(3,6,2)$, dan $(1,0,4)$.

## jawaban

### 1. Luas jajaran genjang dari velttor 

$$
\vec{u}=\left[\begin{array}{l}
1 \\
2
\end{array}\right], \quad \vec{v}=\left[\begin{array}{l}
2 \\
1
\end{array}\right]
$$

Untuk vektor 2D, luas jajaran genjang adalah nilai absolut dari determinan matriks 2x2: 

$$
\text { Luas }=|\vec{u} \times \vec{v}|=\left|\begin{array}{ll}
1 & 2 \\
2 & 1
\end{array}\right|=|(1)(1)-(2)(2)|=|1-4|=3
$$

Jawaban: Luas = 3

### 2. Luas jajaran genjang dari vektor

$$
\begin{gathered}
\vec{u}=\left[\begin{array}{l}
2 \\
0
\end{array}\right], \quad \vec{v}=\left[\begin{array}{l}
0 \\
3
\end{array}\right] \\
\text { Luas }=\left|\begin{array}{ll}
2 & 0 \\
0 & 3
\end{array}\right|=|(2)(3)-(0)(0)|=|6|=6
\end{gathered}
$$

Jawaban: Luas = 6

### 3. Luas segitiga dengan titik-titik sudut

$$
A=(0,0,0), \quad B=(1,3,-1), \quad C=(2,1,1)
$$

Hitung vektor.
$$
\overrightarrow{A B}=B-A=\left[\begin{array}{c}
1 \\
3 \\
-1
\end{array}\right], \quad \overrightarrow{A C}=C-A=\left[\begin{array}{l}
2 \\
1 \\
1
\end{array}\right]
$$

Hitung cross product

$$
\begin{gathered}
\overrightarrow{A B} \times \overrightarrow{A C}=\left|\begin{array}{ccc}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
1 & 3 & -1 \\
2 & 1 & 1
\end{array}\right|=\mathbf{i}(3 \cdot 1-(-1) \cdot 1)-\mathbf{j}(1 \cdot 1-(-1) \cdot 2)+\mathbf{k}(1 \cdot 1-3 \cdot 2) \\
=\mathbf{i}(3+1)-\mathbf{j}(1+2)+\mathbf{k}(1-6)=\left[\begin{array}{c}
4 \\
-3 \\
-5
\end{array}\right]
\end{gathered}
$$

Panjang vektor hasil cross: 

$$
|\overrightarrow{A B} \times \overrightarrow{A C}|=\sqrt{4^2+(-3)^2+(-5)^2}=\sqrt{16+9+25}=\sqrt{50}
$$

Luas segitiga $=1 / 2 \times \mid$ cross product:

$$
\text { Luas }=\frac{1}{2} \sqrt{50}=\frac{1}{2} \cdot 5 \sqrt{2}=\frac{5 \sqrt{2}}{2}
$$

Jawaban: Luas $=\frac{5 \sqrt{2}}{2}$

### 4. Luas segitiga dengan titik-titik sudut 

$$
A=(5,2,-1), \quad B=(3,6,2), \quad C=(1,0,4)
$$

Hitung vektor:

$$
\overrightarrow{A B}=B-A=\left[\begin{array}{c}
-2 \\
4 \\
3
\end{array}\right], \quad \overrightarrow{A C}=C-A=\left[\begin{array}{c}
-4 \\
-2 \\
5
\end{array}\right]
$$

Cross product

$$
\begin{gathered}
\overrightarrow{A B} \times \overrightarrow{A C}=\left|\begin{array}{ccc}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
-2 & 4 & 3 \\
-4 & -2 & 5
\end{array}\right|=\mathbf{i}(4 \cdot 5-3 \cdot(-2))-\mathbf{j}(-2 \cdot 5-3 \cdot(-4))+\mathbf{k}(-2 \cdot(-2)-4 \cdot(-4)) \\
=\mathbf{i}(20+6)-\mathbf{j}(-10+12)+\mathbf{k}(4+16)=\left[\begin{array}{c}
26 \\
-2 \\
20
\end{array}\right]
\end{gathered}
$$

Panjang:

$$
|\overrightarrow{A B} \times \overrightarrow{A C}|=\sqrt{26^2+(-2)^2+20^2}=\sqrt{676+4+400}=\sqrt{1080}
$$

Luas segitiga:

$$
\text { Luas }=\frac{1}{2} \sqrt{1080}=\frac{\sqrt{1080}}{2}
$$

Sederhanakan:

$$
\sqrt{1080}=\sqrt{36 \cdot 30}=6 \sqrt{30}
$$

Jawaban: Luas $=3 \sqrt{30}$