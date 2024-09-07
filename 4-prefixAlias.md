# Prefix dan Alias

perhatikan sintak berikut :

`
SELECT t1.nama_pegawai AS 'nama pegawai', t1.nip AS NIP FROM tabel_pegawai AS t1;
`

* t1 pada nama kolom adalah prefix

* keyword **AS** memberikan nama lain

dua poin diatas dapat digunakan pada nama kolom dan tabel

**prefix** merupakan tambahan identifikasi menggunakan nama tabel ke suatu kolom, yang disambung ke penghubung berupa titik (.)

prefiks sering digunakan terutama jika kita bekerja dengan banyak tabel dengan nama kolom yang sama.

Gambar 1.
![Gambar 1](/gambar1.png)

### Menggunakan alias pada kolom

alias digunakan untuk mempermudah penulisan dan readibility sintaks. Terutama untuk nama kolom yang panjang. Contoh penggunaannya adalah sebagai berikut :

`
SELECT date AS tanggal_akses FROM tabel_visitor;
`

nb : alias tidak dapat digunakan untuk wildcard (*)

untuk menghilangkan alias atau merubah kembali ke nama kolom sebelumnya, dengan cara sebagai berikut :

> kondisi setelah pakai AS :
> SELECT date AS tanggal_akses FROM tabel_visitor;

menjadi ( tinggal hapus AS) :

`
SELECT date tanggal_akses FROM tabel_visitor;
`

### Menggabung prefix dan alias

seperti sintaks diatas, merupakan contoh penggabungan prefix dan alias.

### Menggunakan alias pada tabel

penggunaan **AS** pada tabel digunakan pada umumnya jika nama tabel sangat panjang. Dengan menggunakan alias maka akan menghemat waktu dalam penulisan query.

contoh :

`
SELECT * FROM tabel_visitor AS t1;
`

### prefix dengan alias tabel

Jika kita menggunakan alias pada tabel, maka untuk prefixnya juga menggunakan nama tabel alias tersebut.

bukan nama tabel aslinya.

contoh :

`
SELECT tbl.date as tanggal_akses FROM tabel_visitor AS tbl;
`
