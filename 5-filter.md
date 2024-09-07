# Penggunaan filter WHERE

WHERE digunakan untuk :
* filter dengan kondisi tertentu
* filter dengan nilai tertentu
* dua kondisi dengan AND dan OR


contoh sintaks :

`
SELECT * FROM tabel_visitor WHERE kode_pengunjung = 'Berliani Indah';

![gambar2](/gambar2.png)
`
### Menggunakan operand OR

Untuk menggunakan **OR**, tambahkan pada sintak setelah kondisi dalam WHERE

contoh :

`
SELECT * FROM tabel_visitor WHERE nama_pengunjung = 'Berliani Indah' OR nama_pengunjung = 'Mutiara Ayu' ;
`

### WHERE menggunakan value

sintak sama seperti sebelumnya, hanya saja menggunakan argumen nilai. contohnya sebagai berikut :

`
SELECT * FROM tabel_visitor WHERE umur < 20 ;
`
### Where menggunakan operand AND

seperti sintaks sebelumnya, hanya mengganti operand OR menjadi AND.

data akan ditampilkan jika sejumlah kondisi terpenuhi. jika tidak, maka tidak akan ditampilkan.

contoh :

`
SELECT * FROM tabel_visitor WHERE nama_pengunjung = 'Anisa Yuliastuti' AND umur > 20;
`

berikut contoh sintak dari final projek elearning SELECT :

`
SELECT kode_barang, nama_barang, qty, harga_satuan, qty * harga_satuan AS harga_total FROM tabel_persediaan WHERE harga_total >= 150000 ORDER BY harga_total DESC ;
`