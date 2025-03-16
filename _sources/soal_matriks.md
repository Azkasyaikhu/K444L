## Sistem Persamaan Linear Dengan Menggunakan Invers OBE (Operasi Baris Elementer)

$-7x1-6x2-12x3=-33$ 

$5x1+5x2+7x3=24$

$x1+4x3=5$
    
$A=\begin{bmatrix}-7&-6&-12\\5&5&7\\1&0&4\end{bmatrix}$  
$x=\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}$  
$b=\begin{bmatrix}-33\\24\\5\end{bmatrix}$`

Pertama Gabungkan matriks ( A ) dengan matriks identitas $( I )$ untuk membentuk matriks augmented $( [A | I] )$:


$[A | I] =
\begin{bmatrix}
-7 & -6 & -12 & | 1 & 0 & 0 \\
5 & 5 & 7 & | 0 & 1 & 0 \\
1 & 0 & 4 & | 0 & 0 & 1
\end{bmatrix}$

pakai OBE jadi yang bagian kanan menjadi $( A^{-1} )$.

Lalu kita Ubah Elemen (1,1) Menjadi 1
jadi Baris pertama dibagi dengan (-7):

$\begin{bmatrix}
1 & \frac{6}{7} & \frac{12}{7} & | -\frac{1}{7} & 0 & 0 \\
5 & 5 & 7 & | 0 & 1 & 0 \\
1 & 0 & 4 & | 0 & 0 & 1
\end{bmatrix}$

Lalu Buat Elemen Kolom Pertama (2,1) dan (3,1) Menjadi 0
- Baris kedua: $( R_2 \to R_2 - 5 R_1 )$
- Baris ketiga: $( R_3 \to R_3 - R_1 )$

Hasilnya:

$\begin{bmatrix}
1 & \frac{6}{7} & \frac{12}{7} & | -\frac{1}{7} & 0 & 0 \\
0 & \frac{5}{7} & -\frac{1}{7} & | \frac{5}{7} & 1 & 0 \\
0 & -\frac{6}{7} & \frac{16}{7} & | \frac{1}{7} & 0 & 1
\end{bmatrix}$

Ubah Elemen (2,2) Menjadi 1
Kita bagi baris kedua dengan $( \frac{5}{7} )$:

$\begin{bmatrix}
1 & \frac{6}{7} & \frac{12}{7} & | -\frac{1}{7} & 0 & 0 \\
0 & 1 & -\frac{1}{5} & | 1 & \frac{7}{5} & 0 \\
0 & -\frac{6}{7} & \frac{16}{7} & | \frac{1}{7} & 0 & 1
\end{bmatrix}$

Setelah Itu Buat Elemen Kolom Kedua (1,2) dan (3,2) Menjadi 0
- Baris pertama: $( R_1 \to R_1 - \frac{6}{7} R_2 )$
- Baris ketiga: $( R_3 \to R_3 + \frac{6}{7} R_2 )$

Hasilnya:

$\begin{bmatrix}
1 & 0 & \frac{18}{35} & | -\frac{13}{35} & -\frac{42}{35} & 0 \\
0 & 1 & -\frac{1}{5} & | 1 & \frac{7}{5} & 0 \\
0 & 0 & \frac{22}{35} & | \frac{13}{35} & \frac{42}{35} & 1
\end{bmatrix}$

Ubah Elemen (3,3) Menjadi 1
Kita bagi baris ketiga dengan $( \frac{22}{35} )$:

$\begin{bmatrix}
1 & 0 & \frac{18}{35} & | -\frac{13}{35} & -\frac{42}{35} & 0 \\
0 & 1 & -\frac{1}{5} & | 1 & \frac{7}{5} & 0 \\
0 & 0 & 1 & | \frac{13}{22} & \frac{42}{22} & \frac{35}{22}
\end{bmatrix}$

Buat Elemen Kolom Ketiga (1,3) dan (2,3) Menjadi 0
- Baris pertama: $( R_1 \to R_1 - \frac{18}{35} R_3 )$
- Baris kedua: $( R_2 \to R_2 + \frac{1}{5} R_3 )$

Hasilnya:

$\begin{bmatrix}
1 & 0 & 0 & | -3 & 5 & 2 \\
0 & 1 & 0 & | 2 & 1 & 1 \\
0 & 0 & 1 & | \frac{13}{22} & \frac{21}{11} & \frac{35}{22}
\end{bmatrix}$
Bagian kanan dari matriks ini adalah $( A^{-1} )$.

Langkah 8: Hitung $( x = A^{-1} b )$
Kita kalikan $( A^{-1} )$ dengan $( b )$:

$x = A^{-1} b =
\begin{bmatrix}
-3 & 5 & 2
\end{bmatrix}$

Sehingga diperoleh:

$x_1 = -3, \quad x_2 = 5, \quad x_3 = 2$