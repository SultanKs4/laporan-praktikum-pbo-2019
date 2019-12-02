# Laporan Praktikum #14 - GUI dan Database

## Kompetensi

Setelah menempuh materi percobaan ini, mahasiswa mampu mengenal:

1. Menggunakan paradigma berorientasi objek untuk interaksi dengan database.
2. Membuat backend dan frontend.
3. Membuat form sebagai frontend.

## Ringkasan Materi

Secara umum, tahapan yang akan kita lakukan adalah sebagai berikut:

1. Membuat database dan tabel-tabelnya.
2. Membuat backend yang berisi class-class yang mewakili data yang ada pada database, dan
class helper untuk melakukan eksekusi query database.
3. Membuat frontend yang merupakan antarmuka kepada pengguna. Frontend ini bisa

berbasis teks (console), GUI, web, mobile, dan sebagainya. Library yang digunakan untuk project ini antara lain:

1. JDBC, untuk melakukan interaksi ke database.
2. ArrayList, untuk menampung data hasil query ke database.
3. Swing, untuk membuat tampilan GUI.

## Percobaan

### Percobaan 1

Membuat Database

`Screenshot`

![percobaan 1 ss](img/percobaan1-ss.png)

### Percobaan 2

Membuat Project

`Screenshot`

![percobaan 2 ss](img/percobaan2-ss.png)

### Percobaan 3

Membuat class helper untuk mengeksekusi query SQL.

`Screenshot`

![percobaan 3 ss](img/percobaan3-ss.png)

`Kode Program`

[DBHelper1841720019Sultan.java](../../src/14_GUI_dan_Database/backend/DBHelper1841720019Sultan.java)

### Percobaan 4

Membuat class **Kategori** untuk menghandle CRUD pada tabel kategori.

`Screenshot`

![percobaan 4 ss](img/percobaan4-ss.png)

`Kode Program`

[Kategori1841720019Sultan.java](../../src/14_GUI_dan_Database/backend/Kategori1841720019Sultan.java)

### Percobaan 5

Mencoba backed yang sudah dibuat dengan mengoperasikannya lewat frontend berbasis teks (console). Percobaan ini dapat anda skip jika anda telah yakin bahwa backend yang anda buat sudah berfungsi dengan baik.

`Screenshot`

![percobaan 5 ss](img/percobaan5-ss.png)

`Kode Program`

[TestBackend1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/TestBackend1841720019Sultan.java)

### Percobaan 6

Pada percobaan ini kita akan membuat interface utama untuk program kita yaitu GUI.

* FrmKategori

    `Screenshot`

    ![percobaan 6 ss](img/percobaan6-ss.png)

    ![percobaan 6 ss db](img/percobaan6-ss-db.png)

    `Kode Program`

  * [FrmKategori1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/FrmKategori1841720019Sultan.java)
  * [FrmKategori1841720019Sultan.form](../../src/14_GUI_dan_Database/frontend/FrmKategori1841720019Sultan.form)

Lakukan hal yang sama untuk data **Anggota**!

* Anggota

    `Screenshot`

    ![percobaan 6 ss 2](img/percobaan6-ss2.png)

    `Kode Program`

    [Anggota1841720019Sultan.java](../../src/14_GUI_dan_Database/backend/Anggota1841720019Sultan.java)

* TestBackendAnggota

    `Screenshot`

    ![percobaan 6 ss 3](img/percobaan6-ss3.png)

    `Kode Program`

    [TestBackendAnggota1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/TestBackendAnggota1841720019Sultan.java)

### Percobaan 7

Buat form untuk data Anggota.

* FrmAnggota

    `Screenshot`

    ![percobaan 7 ss](img/percobaan7-ss.png)

    ![percobaan 7 ss db](img/percobaan7-ss-db.png)

    `Kode Program`

  * [FrmAnggota1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/FrmAnggota1841720019Sultan.java)
  * [FrmAnggota1841720019Sultan.form](../../src/14_GUI_dan_Database/frontend/FrmAnggota1841720019Sultan.form)

Untuk data **Buku**, caranya kurang lebih sama seperti data Kategori dan Anggota. Hanya saja yang
berbeda adalah:

* Pemanggilan **getKategori().getIdKategori()** pada query insert dan update untuk mengeset **idkategori** pada tabel buku
* Query select yang melibatkan join table.

Kode lengkap class Buku dapat anda lihat di **Lampiran 1**. Untuk test buku pada **frontend**, bisa anda lihat di **Lampiran 2**.

* Buku

    `Screenshot`

    ![percobaan 7 ss 2](img/percobaan7-ss2.png)

    `Kode Program`

    [Buku1841720019Sultan.java](../../src/14_GUI_dan_Database/backend/Buku1841720019Sultan.java)

* TestBackendBuku

    `Screenshot`

    ![percobaan 7 ss 3](img/percobaan7-ss3.png)

    `Kode Program`

    [TestBackendBuku1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/TestBackendBuku1841720019Sultan.java)

### Percobaan 8

Membuat GUI untuk data Buku, yang dilengkapi dengan combo box untuk memilih kategori, yang terhubung dengan tabel kategori.

* FrmBuku

    `Screenshot`

    ![percobaan 8 ss](img/percobaan8-ss.png)

    ![percobaan 8 ss db](img/percobaan8-ss-db.png)

    `Kode Program`

  * [FrmBuku1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/FrmBuku1841720019Sultan.java)
  * [FrmBuku1841720019Sultan.form](../../src/14_GUI_dan_Database/frontend/FrmBuku1841720019Sultan.form)

## Tugas

1. Buatlah class **Peminjaman**.

    * Peminjaman

        `Screenshot`

        ![tugas 1 ss](img/tugas1-ss.png)

        `Kode Program`

        [Peminjaman1841720019Sultan.java](../../src/14_GUI_dan_Database/backend/Peminjaman1841720019Sultan.java)

    * TestBackendPeminjaman

        `Screenshot`

        ![tugas 1 ss 2](img/tugas1-ss2.png)

        `Kode Program`

        [TestBackendPeminjaman1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/TestBackendPeminjaman1841720019Sultan.java)

2. Buatlah class **FrmPeminjaman** dan susun sebagai berikut:

    ![Soal tugas2](img/tugas2-soal.png)

    `Screenshot`

    ![tugas 2 ss](img/tugas2-ss.png)

    `Kode Program`

    * [FrmPeminjaman1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/FrmPeminjaman1841720019Sultan.java)
    * [FrmPeminjaman1841720019Sultan.form](../../src/14_GUI_dan_Database/frontend/FrmPeminjaman1841720019Sultan.form)

3. Atur kode program agar dapat menangani transaksi peminjaman dan pengembalian

`Screenshot`

![tugas 3 ss](img/tugas3-ss.png)

![tugas 3 ss db](img/tugas3-ss-db.png)

`Kode Program`

* [FrmPeminjaman1841720019Sultan.java](../../src/14_GUI_dan_Database/frontend/FrmPeminjaman1841720019Sultan.java)
* [FrmPeminjaman1841720019Sultan.form](../../src/14_GUI_dan_Database/frontend/FrmPeminjaman1841720019Sultan.form)

## Kesimpulan

1. Saya mampu menggunakan paradigma berorientasi objek untuk interaksi dengan database.
2. Saya mampu membuat backend dan frontend.
3. Saya mampu membuat form sebagai frontend.

## Pernyataan Diri

Saya menyatakan isi tugas, kode program, dan laporan praktikum ini dibuat oleh saya sendiri. Saya tidak melakukan plagiasi, kecurangan, menyalin/menggandakan milik orang lain.

Jika saya melakukan plagiasi, kecurangan, atau melanggar hak kekayaan intelektual, saya siap untuk mendapat sanksi atau hukuman sesuai peraturan perundang-undangan yang berlaku.

Ttd,

***Sultan Achmad Qum Masykuro NS***
