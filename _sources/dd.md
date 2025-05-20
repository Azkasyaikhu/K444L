# Eigenvalues dan Eigenvector

##1. Definisi Eigenvalues dan Eigenvector

1. Eigenvalue adalah skala (angka) yang menyatakan berapa kali panjang eigenvector berubah karena transformasi itu.
2. Eigenvector adalah vektor spesial yang tidak berubah arah saat transformasi—panjangnya bisa berubah (diperbesar atau diperkecil), tapi arahnya tetap.

##2. Mencari Eigenvalues dan Eigenvector menggikan Polynomial Carakteristik 
### 1. Matriks A

Pertama-tama Bentuk $A - \lambda I$

Kita kurangkan $\lambda$ dari diagonal (karena $I$ adalah matriks identitas):

$$
A - \lambda I =
\begin{bmatrix}
3 - \lambda & 0 \\
0 & 3 - \lambda
\end{bmatrix}
$$

lalu Determinan dari $A - \lambda I$

$$
\det(A - \lambda I) = (3 - \lambda)(3 - \lambda) = (3 - \lambda)^2
$$

Selanjutnya Polinomial Karakteristik

$$
(3 - \lambda)^2 = 0
\Rightarrow \lambda = 3 \quad \text{(dengan multiplikasi 2)}
$$

lalu cari Eigenvector

Selesaikan:

$$
(A - 3I)\vec{v} = \vec{0}
\Rightarrow
\begin{bmatrix}
0 & 0 \\
0 & 0
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
= 
\begin{bmatrix}
0 \\
0
\end{bmatrix}
$$

Sistem ini memberikan solusi:

$$
x \text{ bebas}, \quad y \text{ bebas} \Rightarrow
\vec{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}, \quad \text{dengan } (x,y) \ne (0,0)
$$

Artinya, semua vektor tak nol adalah eigenvector untuk $\lambda = 3$.

### 2. Matriks B

Pertama Bentuk $B - \lambda I$

$$
B - \lambda I =
\begin{bmatrix}
-2 - \lambda & 0 \\
0 & 4 - \lambda
\end{bmatrix}
$$

lalu kita cari Determinan

$$
\det(B - \lambda I) = (-2 - \lambda)(4 - \lambda)
$$

Selanjutnya Polinomial Karakteristik

$$
(-2 - \lambda)(4 - \lambda) = 0
\Rightarrow \lambda_1 = -2, \quad \lambda_2 = 4
$$

Lalu Cari Eigenvector untuk $\lambda = -2$

$$
B - (-2)I = B + 2I =
\begin{bmatrix}
0 & 0 \\
0 & 6
\end{bmatrix}
$$

Selesaikan:

$$
\begin{bmatrix}
0 & 0 \\
0 & 6
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
=
\begin{bmatrix}
0 \\
0
\end{bmatrix}
\Rightarrow
6y = 0 \Rightarrow y = 0
\Rightarrow x \text{ bebas}
$$

Jadi, eigenvectornya:

$$
\vec{v}_1 =
\begin{bmatrix}
x \\
0
\end{bmatrix}, \quad x \ne 0
\Rightarrow \vec{v}_1 = x \begin{bmatrix} 1 \\ 0 \end{bmatrix}
$$

Ambil $x = 1$, maka:

$$
\vec{v}_1 = \begin{bmatrix} 1 \\ 0 \end{bmatrix}
$$

lalu Cari Eigenvector untuk $\lambda = 4$

$$
B - 4I =
\begin{bmatrix}
-6 & 0 \\
0 & 0
\end{bmatrix}
$$

Selesaikan:

$$
\begin{bmatrix}
-6 & 0 \\
0 & 0
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
=
\begin{bmatrix}
0 \\
0
\end{bmatrix}
\Rightarrow
-6x = 0 \Rightarrow x = 0
\Rightarrow y \text{ bebas}
$$

Jadi, eigenvectornya:

$$
\vec{v}_2 = \begin{bmatrix}
0 \\
y
\end{bmatrix}, \quad y \ne 0
\Rightarrow \vec{v}_2 = y \begin{bmatrix} 0 \\ 1 \end{bmatrix}
$$

Ambil $y = 1$, maka:

$$
\vec{v}_2 = \begin{bmatrix} 0 \\ 1 \end{bmatrix}
$$

