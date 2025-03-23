# Determinan Matriks
## Definisi
determinan adalah fungsi yang mengaitkan suatu matriks persegi A dengan sebuah bilangan real (skalar)


## Fungsi Determinan
1. Digunakan untuk menentukan apakah suatu matriks memiliki invers (det(𝐴)≠0).
2. Digunakan dalam perhitungan invers matriks melalui rumus:


$$
A^{-1} = \frac{1}{\det(A)} \cdot \text{adj}(A)
$$




## Sifat-Sifat Determinan
1. Determinan Matriks Identitas:
det(𝐼)=1, di mana 𝐼 adalah matriks identitas.
2. Baris atau Kolom Nol:
Jika ada baris atau kolom yang semuanya nol, maka det(𝐴)=0.
3.Matriks Singular:
Jika det(𝐴)=0, maka matriks 𝐴 disebut singular (tidak memiliki invers).
4.Pertukaran Baris/Kolom:
Jika dua baris atau kolom dipertukarkan, determinan berubah tanda.
5.Kelipatan Baris/Kolom:
Jika satu baris atau kolom dikalikan dengan skalar 𝑘, maka determinan menjadi 𝑘⋅det(𝐴).

## Metode Sarrus (Hanya untuk Matriks 3 x 3)
Metode ini hanya berlaku untuk matriks berukuran 3×3.
Langkah-langkah:1. Tuliskan ulang dua kolom pertama di sebelah kanan matriks.2. Jumlahkan hasil perkalian diagonal utama, lalu kurangi hasil perkalian diagonal sekunder.

Rumus
 det(𝐴 )=(𝑎_11 𝑎_22 𝑎_33+𝑎_12 𝑎_23 𝑎_31+𝑎_13 𝑎_21 𝑎_32 )−(𝑎_13 𝑎_22 𝑎_31+𝑎_11 𝑎_23 𝑎_32+𝑎_12 𝑎_21 𝑎_33 )
 

### Minor Matriks

#### Definisi
Minor matriks adalah bagian matriks yang tersisa setelah mengecualikan baris dan kolom yang berisi elemen tertentu. Minor matriks dapat dihitung dengan menghitung determinan matriks persegi. 

Contoh:
 Diberikan matriks:
    
$$
    A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix}
    $$
    
Minor dari elemen $a_{11}$ adalah:
    
$$
    M_{11} = \det \begin{bmatrix} 5 & 6 \\ 8 & 9 \end{bmatrix} = (5 \cdot 9) - (6 \cdot 8) = 45 - 48 = -3
    $$



### Cofactor Matriks
Kofaktor matriks adalah nilai yang diperoleh dengan mengalikan minor elemen matriks dengan \((-1)^{i+j}\), di mana \(i\) adalah nomor baris dan \(j\) adalah nomor kolom elemen tersebut. 

Contoh:
Menggunakan matriks yang sama:

$$A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix}$$

Minor dari elemen $a_{11}$ adalah:

$$
C_{11} = (-1)^{1+1} \cdot M_{11} = 1 \cdot (-3) = -3$$


### Mencari Determinan Dengan konsep Minor dan Cofactor Matriks.

### Contoh Matriks 3x3
Tentukan determinan matriks A berikut menggunakan metode minor dan kofaktor:
$$A = \begin{pmatrix}
2 & 1 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix}$$

Penyelesaian :
 1.Tentukan Minor
 
 Minor dari elemen a<sub>ij</sub>, dilambangkan dengan M<sub>ij</sub>, adalah determinan dari submatriks yang diperoleh dengan menghilangkan baris ke-i dan kolom ke-j dari matriks A.

M<sub>11</sub> = | 5 6 | = (59) - (68) = 45 - 48 = -3 | 8 9 |
M<sub>12</sub> = | 4 6 | = (49) - (67) = 36 - 42 = -6 | 7 9 |
M<sub>13</sub> = | 4 5 | = (48) - (57) = 32 - 35 = -3 | 7 8 |
M<sub>21</sub> = | 1 3 | = (19) - (38) = 9 - 24 = -15 | 8 9 |
M<sub>22</sub> = | 2 3 | = (29) - (37) = 18 - 21 = -3 | 7 9 |
M<sub>23</sub> = | 2 1 | = (28) - (17) = 16 - 7 = 9 | 7 8 |
M<sub>31</sub> = | 1 3 | = (16) - (35) = 6 - 15 = -9 | 5 6 |
M<sub>32</sub> = | 2 3 | = (26) - (34) = 12 - 12 = 0 | 4 6 |
M<sub>33</sub> = | 2 1 | = (25) - (14) = 10 - 4 = 6 | 4 5 |

2.  Tentukan Kofaktor

Kofaktor dari elemen a<sub>ij</sub>, dilambangkan dengan C<sub>ij</sub>, dihitung dengan rumus:

C<sub>ij</sub> = (-1)<sup>i+j</sup> * M<sub>ij</sub>

C<sub>11</sub> = (-1)<sup>1+1</sup> * M<sub>11</sub> = 1 * (-3) = -3
C<sub>12</sub> = (-1)<sup>1+2</sup> * M<sub>12</sub> = -1 * (-6) = 6
C<sub>13</sub> = (-1)<sup>1+3</sup> * M<sub>13</sub> = 1 * (-3) = -3
C<sub>21</sub> = (-1)<sup>2+1</sup> * M<sub>21</sub> = -1 * (-15) = 15
C<sub>22</sub> = (-1)<sup>2+2</sup> * M<sub>22</sub> = 1 * (-3) = -3
C<sub>23</sub> = (-1)<sup>2+3</sup> * M<sub>23</sub> = -1 * (9) = -9
C<sub>31</sub> = (-1)<sup>3+1</sup> * M<sub>31</sub> = 1 * (-9) = -9
C<sub>32</sub> = (-1)<sup>3+2</sup> * M<sub>32</sub> = -1 * (0) = 0
C<sub>33</sub> = (-1)<sup>3+3</sup> * M<sub>33</sub> = 1 * (6) = 6

3.Hitung Determinan

Determinan matriks A dapat dihitung dengan mengalikan elemen-elemen pada baris atau kolom mana pun dengan kofaktornya, lalu menjumlahkan hasilnya. Misalnya, menggunakan baris pertama:

det(A) = a<sub>11</sub> * C<sub>11</sub> + a<sub>12</sub> * C<sub>12</sub> + a<sub>13</sub> * C<sub>13</sub>
= 2 * (-3) + 1 * 6 + 3 * (-3)
= -6 + 6 - 9
= -9

Jadi, determinan matriks A adalah -9.

### Contoh Matriks 4x4 :
Tentukan determinan matriks B berikut menggunakan metode minor dan kofaktor:

$$B = \begin{pmatrix}
1 & 2 & 3 & 4 \\
0 & 1 & 2 & 3 \\
5 & 6 & 0 & 1 \\
2 & 4 & 1 & 0
\end{pmatrix}$$

Penyelesaian :

1. Pilih Baris atau Kolom

Memilih baris atau kolom mana saja untuk menghitung determinan. Untuk mempermudah perhitungan, kita pilih baris kedua karena memiliki elemen nol.

2. Tentukan Minor

- M<sub>21</sub> = determinan dari submatriks 3x3 yang diperoleh dengan menghilangkan baris ke-2 dan kolom ke-1:
$$\begin{pmatrix}
2 & 3 & 4 \\
6 & 0 & 1 \\
4 & 1 & 0
\end{pmatrix}$$
M<sub>21</sub> = 2(0-1) - 3(0-4) + 4(6-0) = -2 + 12 + 24 = 34
- M<sub>22</sub> = determinan dari submatriks 3x3 yang diperoleh dengan menghilangkan baris ke-2 dan kolom ke-2:
$$\begin{pmatrix}
1 & 3 & 4 \\
5 & 0 & 1 \\
2 & 1 & 0
\end{pmatrix}$$
M<sub>22</sub> = 1(0-1) - 3(0-2) + 4(5-0) = -1 + 6 + 20 = 25
- M<sub>23</sub> = determinan dari submatriks 3x3 yang diperoleh dengan menghilangkan baris ke-2 dan kolom ke-3:
$$\begin{pmatrix}
1 & 2 & 4 \\
5 & 6 & 1 \\
2 & 4 & 0
\end{pmatrix}$$
M<sub>23</sub> = 1(0-4) - 2(0-2) + 4(20-12) = -4 + 4 + 32 = 32
- M<sub>24</sub> = determinan dari submatriks 3x3 yang diperoleh dengan menghilangkan baris ke-2 dan kolom ke-4:
$$\begin{pmatrix}
1 & 2 & 3 \\
5 & 6 & 0 \\
2 & 4 & 1
\end{pmatrix}$$
M<sub>24</sub> = 1(6-0) - 2(5-0) + 3(20-12) = 6 - 10 + 24 = 20

3. Tentukan Kofaktor
C<sub>21</sub> = (-1)<sup>2+1</sup> * M<sub>21</sub> = -1 * 34 = -34
C<sub>22</sub> = (-1)<sup>2+2</sup> * M<sub>22</sub> = 1 * 25 = 25
C<sub>23</sub> = (-1)<sup>2+3</sup> * M<sub>23</sub> = -1 * 32 = -32
C<sub>24</sub> = (-1)<sup>2+4</sup> * M<sub>24</sub> = 1 * 20 = 20

4.  Hitung Determinan

det(B) = b<sub>21</sub> * C<sub>21</sub> + b<sub>22</sub> * C<sub>22</sub> + b<sub>23</sub> * C<sub>23</sub> + b<sub>24</sub> * C<sub>24</sub>
= 0 * (-34) + 1 * 25 + 2 * (-32) + 3 * 20
= 0 + 25 - 64 + 60
= 21

Jadi, determinan matriks B adalah 21.

### Contoh Matriks 5x5 :

Tentukan determinan matriks C berikut menggunakan metode minor dan kofaktor:
$$C = \begin{pmatrix}
1 & 0 & 2 & 0 & 1 \\
2 & 1 & 0 & 3 & 0 \\
0 & 2 & 1 & 0 & 2 \\
1 & 0 & 0 & 1 & 0 \\
0 & 1 & 2 & 0 & 1
\end{pmatrix}$$

1.  Pilih Baris atau Kolom
Kita pilih baris ke-4 karena memiliki banyak elemen nol, yang akan menyederhanakan perhitungan.

2. Tentukan Minor
M<sub>41</sub>: Determinan dari submatriks 4x4 yang diperoleh dengan menghilangkan baris ke-4 dan kolom ke-1.
M<sub>42</sub>: Determinan dari submatriks 4x4 yang diperoleh dengan menghilangkan baris ke-4 dan kolom ke-2.
M<sub>43</sub>: Determinan dari submatriks 4x4 yang diperoleh dengan menghilangkan baris ke-4 dan kolom ke-3.
M<sub>44</sub>: Determinan dari submatriks 4x4 yang diperoleh dengan menghilangkan baris ke-4 dan kolom ke-4.
M<sub>45</sub>: Determinan dari submatriks 4x4 yang diperoleh dengan menghilangkan baris ke-4 dan kolom ke-5.
Perhitungan minor 4x4 ini sendiri memerlukan proses yang panjang dan melibatkan perhitungan minor 3x3 dan 2x2.

3. Tentukan Kofaktor
C<sub>41</sub> = (-1)<sup>4+1</sup> * M<sub>41</sub> = -M<sub>41</sub>
C<sub>42</sub> = (-1)<sup>4+2</sup> * M<sub>42</sub> = M<sub>42</sub>
C<sub>43</sub> = (-1)<sup>4+3</sup> * M<sub>43</sub> = -M<sub>43</sub>
C<sub>44</sub> = (-1)<sup>4+4</sup> * M<sub>44</sub> = M<sub>44</sub>
C<sub>45</sub> = (-1)<sup>4+5</sup> * M<sub>45</sub> = -M<sub>45</sub>

4. Hitung Determinan
det(C) = c<sub>41</sub> * C<sub>41</sub> + c<sub>42</sub> * C<sub>42</sub> + c<sub>43</sub> * C<sub>43</sub> + c<sub>44</sub> * C<sub>44</sub> + c<sub>45</sub> * C<sub>45</sub>

det(C) = (1 * C<sub>41</sub>) + (0 * C<sub>42</sub>) + (0 * C<sub>43</sub>) + (1 * C<sub>44</sub>) + (0 * C<sub>45</sub>)

det(C) = C<sub>41</sub> + C<sub>44</sub>

Penyelesaian Perhitungan Minor 4x4:

Untuk menyelesaikan perhitungan matriks 5x5 ini, kita harus mencari nilai dari C<sub>41</sub> dan C<sub>44</sub>, yang artinya kita perlu mencari nilai dari M<sub>41</sub> dan M<sub>44</sub>.

- M<sub>41</sub> = determinan dari :
$$\begin{pmatrix}
0 & 2 & 0 & 1 \\
1 & 0 & 3 & 0 \\
2 & 1 & 0 & 2 \\
1 & 2 & 0 & 1
\end{pmatrix}$$

- M<sub>44</sub> = determinan dari :
$$\begin{pmatrix}
1 & 0 & 2 & 1 \\
2 & 1 & 0 & 0 \\
0 & 2 & 1 & 2 \\
0 & 1 & 2 & 1
- [ ] - [ ] - [ ] \end{pmatrix}$$

Setelah melakukan perhitungan determinan 4x4, dengan cara yang sama seperti 3x3, akan didapatkan hasil dari M<sub>41</sub> dan M<sub>44</sub>, dan kemudian bisa mendapatkan hasil dari C<sub>41</sub> dan C<sub>44</sub>.