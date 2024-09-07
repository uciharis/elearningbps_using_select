# SELECT statement

SELECT adalah perintah DML yang digunakan untuk mengambil data dari tabel database.

SELECT digunakan untuk menentukan kolom yang ingin diambil.

SELECT tidak berdiri sendiri, argumennya diikuti FROM. Formatnya adalah sebagai berikut :

> SELECT nama_kolom1, nama_kolom2, ...

> FROM nama_tabel1, ...

> WHERE kondisi1, kondisi2, ...

Gambar 1.
![Gambar 1](/gambar1.png)

Berikut ditampilkan tabel dari database suatu instansi yang berisi 10 data pegawai.

### Mengambil seluruh kolom dalam suatu Tabel

tanda bintang (*) disebut sebagai wildcard, untuk merujuk ke seluruh kolom.

tanda titik koma (;) adalah penanda mengakhiri perintah pada SQL.

Untuk mengambil seluruh kolom pada tabel_pegawai, sintaknya sebagai berikut :

`
SELECT * FROM tabel_pegawai
`

### Mengambil satu kolom dari tabel

mengambil semua kolom akan membutuhkan waktu yang lama. Selain itu, tidak semua kolom kita perlukan. Maka dari itu pengambilannya adalah sebagai berikut :

> SELECT nama_kolom FROM nama_table ;

berdasarkan gambar 1, misal kita mengambil data nama_pegawai. maka sintaksnya adalah :

`
SELECT nama_pegawai FROM tabel_pegawai;
`

### Mengambil lebih dari 1 kolom pada suatu tabel

Sintaknya sama, hanya berisi tambahan beberapa kolom saja. Misalkan kita akan mengambil kolom nama_pegawai dan jabatan, maka :

`
SELECT nama_pegawai, jabatan FROM tabel_pegawai;
`

### membatasi pengambilan jumlah row

untuk membatasi jumlah row yang ditampilkan, tambahkan LIMIT (jumlah baris). contohnya :

`
SELECT nama_pegawai FROM tabel_pegawai LIMIT 4;
`

### Penggunaan SELECT DISTINCT

digunakan untuk menampilkan data yang unik (tidak duplikat). contoh penggunaan :

`
SELECT DISTINCT nama_pegawai, jenis_kelamin FROM tabel_pegawai;
`

