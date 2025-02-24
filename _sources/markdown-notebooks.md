## Penyelesaian Sistem Persamaan liniear
Penyelesaian sistem persamaan linear bergantung pada jumlah variabel dan jumlah persamaan.

Berikut beberapa metode penyelesaiannya :
1.Substitusi
Salah satu persamaan diubah sehingga salah satu variabel diekspresikan dalam bentuk variabel lain, lalu disubstitusikan ke dalam persamaan kedua.

2.Eliminasi

Melibatkan penjumlahan atau pengurangan persamaan untuk menghilangkan satu variabel, sehingga sistem dapat diselesaikan secara bertahap.



3. Metode Matriks (Eliminasi Gauss/Jordan, Invers Matriks)

Sistem ditulis dalam bentuk matriks dan diselesaikan menggunakan operasi baris elementer atau invers matriks
### Operasi Baris Elementer
Operasi Baris Elementer (OBE) adalah teknik manipulasi baris pada matriks untuk menyelesaikan sistem persamaan linear. OBE digunakan dalam metode Eliminasi Gauss dan Gauss-Jordan untuk mengubah matriks ke bentuk eselon baris atau eselon tereduksi.

Tiga Jenis Operasi Baris Elementer:

1. Pertukaran Baris (Row Swapping)

Menukar dua baris dalam matriks.

Contoh: Tukar baris ke-1 dan ke-2 → 



2. Perkalian Baris dengan Skalar (Scaling)

Mengalikan suatu baris dengan bilangan bukan nol.

Contoh: Kalikan baris ke-2 dengan 3 → 



3. Penjumlahan atau Pengurangan Baris (Row Addition/Subtraction)

Menjumlahkan atau mengurangkan kelipatan suatu baris ke baris lain.

Contoh:  (mengurangi dua kali baris pertama dari baris kedua)




Contoh Penerapan OBE:

Misalkan kita memiliki sistem persamaan:

\begin{cases}
x + 2y = 5 \\
3x + 4y = 11
\end{cases}

Langkah 1: Tuliskan dalam Matriks Augmented

\begin{bmatrix} 
1 & 2 & | 5 \\ 
3 & 4 & | 11
\end{bmatrix}

Langkah 2: Eliminasi x dari Baris 2
Lakukan operasi:
R_2 \to R_2 - 3R_1

Hasil:

\begin{bmatrix} 
1 & 2 & | 5 \\ 
0 & -2 & | -4
\end{bmatrix}

Langkah 3: Ubah Elemen Pivot Menjadi 1
Bagi baris kedua dengan -2:

R_2 \to \frac{R_2}{-2}

Hasil:

\begin{bmatrix} 
1 & 2 & | 5 \\ 
0 & 1 & | 2
\end{bmatrix}

Langkah 4: Eliminasi y dari Baris 1
Lakukan:

R_1 \to R_1 - 2R_2

Hasil:

\begin{bmatrix} 
1 & 0 & | 1 \\ 
0 & 1 & | 2
\end{bmatrix}

### Eleminasi Gauss
Eliminasi Gauss adalah metode untuk menyelesaikan sistem persamaan linear dengan mengubah matriks augmented menjadi bentuk eselon baris menggunakan operasi baris elementer (OBE).

Berikut beberapa contoh soal eleminasi gauss 


Contoh Soal 1
Selesaikan dengan menggunakan Eleminasi Gauss

$$
\begin{array}{cc}
x_1+2_x2+3x_3z&=6\\
2x_1+4x_2+6x_12&=4\\
x_3-x_2&=2
\end{array}
$$



Contol Soal 2

$$
\begin{array}{cc}
x_1+x_2+x_3&=3\\
2x_1+x_3&=5\\
x_1+2x_2&=3\\
\end{array}
$$

Contoh Soal 3


$$
\begin{array}{cc}
2x_1+2x_2&=4\\
x_1+x_2&=2\\
\end{array}
$$

Penyelesaian
![image](https://hackmd.io/_uploads/SkINBUF51l.png)


Contoh soal 4


$$
\begin{array}{cc}
x_1+x_2&=5\\
x_1+2x_3&=6\\
\end{array}
$$

Penyelesaian
![image](https://hackmd.io/_uploads/S1HPS8Fcyg.png)


### Langkah langkah menyelesaikan Eliminasi Gauss

Langkah 1: Tuliskan dalam Bentuk Matriks Augmented

Misalkan sistem persamaan linear diberikan sebagai:

\begin{cases}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b_1 \\
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b_2 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m
\end{cases}

\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} & | b_1 \\
a_{21} & a_{22} & \dots & a_{2n} & | b_2 \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & | b_m
\end{bmatrix}


---

Langkah 2: Gunakan OBE untuk Membentuk Eselon Baris

Lakukan operasi baris elementer untuk mengubah matriks ke bentuk eselon baris:

1. Pilih Elemen Pivot

Pilih elemen pertama dalam kolom pertama sebagai pivot (elemen utama).

Jika pivot = 0, tukar baris dengan baris lain yang memiliki nilai tidak nol pada kolom tersebut.



2. Buat Elemen di Bawah Pivot Menjadi Nol

Untuk setiap baris di bawah pivot, lakukan operasi:




R_j \to R_j - \frac{a_{j1}}{a_{11}} R_1

3. Ulangi untuk Semua Kolom

Proses ini berlanjut hingga semua elemen di bawah diagonal utama menjadi nol, sehingga terbentuk matriks eselon baris.





---

Langkah 3: Gunakan Substitusi Mundur untuk Menyelesaikan Persamaan

Setelah matriks berbentuk eselon baris, selesaikan nilai variabel dari bawah ke atas (substitusi mundur).

Jika matriks berbentuk eselon baris tereduksi, solusi langsung diperoleh tanpa perlu substitusi mundur.