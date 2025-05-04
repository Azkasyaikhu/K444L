# Pembuktian Transformasi Rotasi Bidang

Kita ingin membuktikan bahwa transformasi linier $T: \mathbb{R}^2 \to \mathbb{R}^2$ yang merepresentasikan rotasi berlawanan arah jarum jam sebesar sudut $\theta$, bisa dinyatakan dengan matriks:

$$
A = 
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
$$

## Langkah-langkah Pembuktian

1. Misalkan kita punya vektor $\mathbf{v} = (x, y)$. Kita bisa ubah ke bentuk koordinat polar:

$$
\mathbf{v} = (x, y) = (r \cos \alpha, r \sin \alpha)
$$

Di mana:
- $r$ adalah panjang dari vektor $\mathbf{v}$
- $\alpha$ adalah sudut antara vektor $\mathbf{v}$ dan sumbu-x positif

2. Jika vektor tersebut diputar sebesar $\theta$, maka posisinya menjadi:

$$
\mathbf{v'} = (r \cos(\alpha + \theta),\ r \sin(\alpha + \theta))
$$

3. Gunakan identitas trigonometri sudut jumlah:

$$
\cos(\alpha + \theta) = \cos \alpha \cos \theta - \sin \alpha \sin \theta
$$
$$
\sin(\alpha + \theta) = \sin \alpha \cos \theta + \cos \alpha \sin \theta
$$

Maka:

$$
\mathbf{v'} = r 
\begin{bmatrix}
\cos \alpha \cos \theta - \sin \alpha \sin \theta \\
\sin \alpha \cos \theta + \cos \alpha \sin \theta
\end{bmatrix}
$$

4. Karena $x = r \cos \alpha$ dan $y = r \sin \alpha$, maka:

$$
\mathbf{v'} = 
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

Artinya, rotasi memang dapat direpresentasikan oleh matriks di atas.
