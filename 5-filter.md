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

### Filter menggunakan value

sintak sama seperti sebelumnya, hanya saja menggunakan argumen nilai. contohnya sebagai berikut :

`
SELECT * FROM tabel_visitor WHERE umur < 20;
`
