---
title: cross_dot

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