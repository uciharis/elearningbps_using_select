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

