# Sistem Persamaan Linier
## Definisi Persamaan Linier
Sistem persamaan linear bisa diartikan sebagai suatu persamaan aljabar. Dimana persamaan linear sendiri memiliki karakteristik pada setiap sukunya mengandung konstanta atau perkalian konstanta dengan variabel tunggal.

Rumus atau bentuk umumnya adalah 
ax + by = c, atau ax + by + c = 0.

Keterangan:
a = koefisien dari x

b = koefisien dari y

x dan y = variabel

c = konstanta

Sifat - sifat persamaan linear :
1.Penjumlahan dan pengurangan bilangan kedua ruas tak akan mengubah persamaan nilai.
2.Perkalian dan pembagian bilangan kedua ruas tidak mengubah nilai persamaan
3.Nilai persamaan tidak berubah jika kedua ruas ditambah atau dikurangi bilangan yang sama.
4.Suatu persamaan jika dipindah ruas maka penjumlahan berubah jadi pengurangan, perkalian berubah menjadi pembagian, dan sebaliknya.

Berikut contoh penerapan sistem persamaan linear dua variabel dalam soal matematika:

Jumlah dua bilangan adalah 15, dan selisih kedua bilangan tersebut adalah 3. Tentukan kedua bilangan tersebut.

Langkah 1 :
- Misalkan bilangan pertama adalah x dan bilangan kedua adalah y.
- Dari informasi soal, kita dapatkan dua persamaan:
x + y = 15 (persamaan 1)
x - y = 3 (persamaan 2)

Langkah 2 :
- Pilih persamaan 2 (x - y = 3) karena lebih mudah untuk diubah bentuknya.
- Nyatakan x dalam bentuk y:
  - x = y + 3 (persamaan 3)

Langkah 3 :
- Substitusikan nilai x dari persamaan 3 (x = y + 3) ke persamaan 1 (x + y = 15):
- (y + 3) + y = 15

Langkah 4 :
- Sederhanakan persamaan:
- 2y + 3 = 15
- 2y = 12
- y = 6

Langkah 5 :
- Substitusikan nilai y = 6 ke persamaan 3 (x = y + 3) untuk mendapatkan nilai x:
- x = 6 + 3
- x = 9

Kesimpulan :
- Jadi, kedua bilangan tersebut adalah 9 dan 6.


## Solusi Persamaan Linier
Dalam memecahkan Persamaan linear terdapat beberapa solusi untuk dapat menyelesaikan persoalan tersebut. Berikut beberapa contoh metode : 

### Metode eliminasi
Metode ini bekerja dengan care mengeliminasi (menghilangkan) variabel-variabel di dalam sistem persamaan hingga hanya satu variabel yang tertinggal.

Pertama-tama, lihat persamaan-persamaan yang ada dan coba cari dua persamaan yang mempunyai koefisien yang sama (baik positif maupun negatif) untuk variabel yang sama. Misalnya, lihat persamaan (1) dan (3).Koefisien untuk y adalah 1 dan −1 untuk masing-masing persamaan. Kita dapat menjumlah kedua persamaan ini untuk menghilangkan y dan kita mendapatkan persamaan (4).

![Screenshot 2025-02-18 101749](https://hackmd.io/_uploads/rkN63OWq1l.png)

Perhatikan bahwa persamaan (4) terdiri atas variabel x dan z. Sekarang kita perlu persamaan lain yang terdiri atas variabel yang sama dengan persamaan(4).Untuk mendapatkan persamaan ini, kita akan menghilangkan y dari persamaan (1)dan (2). Dalam persamaan (1) dan (2), koefisien untuk y adalah 1 dan 3 masing-masing. Untuk menghilangkan y, kita kalikan persamaan (1) dengan 3 lalu mengurangkan persamaan (2) dari persamaan (1).

![Screenshot 2025-02-18 103003](https://hackmd.io/_uploads/r1AAA_b51x.png)

Dengan persamaan (4) dan (5), mari kita coba untuk menghilangkan z.

![Screenshot 2025-02-18 103250](https://hackmd.io/_uploads/rkkFyFW91e.png)

Dari persamaan (6) kita dapatkan x = 2. Sekarang kita bisa subtitusikan (masukkan) nilai dari x ke persamaan (4) untuk mendapatkan nilai z.

![Screenshot 2025-02-18 103434](https://hackmd.io/_uploads/H1001YW9ye.png)

Akhirnya, kita substitusikan (masukkan) nila dari x dan z ke persamaan (1) untuk mendapatkan y.

![Screenshot 2025-02-18 103559](https://hackmd.io/_uploads/SyZElKb5Jx.png)

Jadi solusi sistem persamaan linier di atas adalah x = 2, y = 3, z = 4.

### Eliminasi Gauss / Eliminasi Gauss-Jordan
Sistem persamaan liniear yang terdiri atas persamaan-persamaan (1), (2) dan (3) dapat juga dinyatakan dalam bentuk matriks teraugmentasi seperti berikut

![Screenshot 2025-02-18 103827](https://hackmd.io/_uploads/HyhplY-5yg.png)

Dengan melakukan serangkaian operasi baris (Eliminasi Gauss), kita dapat menyederhanakan matriks di atas untuk menjadi matriks Eselon-baris.

![Screenshot 2025-02-18 103919](https://hackmd.io/_uploads/ryvgWFbcye.png)

Kemudian kita bisa substitusikan kembali nilai-nilai yang kita dapat untuk mencari nilai dari semua variabel. Atau, kita juga bisa meneruskan dengan serangkaian operasi baris lagi sehingga matriks di atas menjadi matriks yang Eselon-baris tereduksi (dengan menggunakan Eliminasi Gauss-Jordan).

![Screenshot 2025-02-18 104001](https://hackmd.io/_uploads/HyX7-K-5kl.png)

Dengan melakukan operasi Eliminasi Gauss-Jordan, kita mendapatkan solusi dari sistem persamaan linier di atas pada kolom terakhir: 
x = 2, y = 3, z = 4 .