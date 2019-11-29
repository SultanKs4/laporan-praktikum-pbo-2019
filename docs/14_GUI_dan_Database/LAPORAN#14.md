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

### Percobaan 2

Membuat Project

### Percobaan 3

Membuat class helper untuk mengeksekusi query SQL.

### Percobaan 4

Membuat class **Kategori** untuk menghandle CRUD pada tabel kategori.

### Percobaan 5

Mencoba backed yang sudah dibuat dengan mengoperasikannya lewat frontend berbasis teks (console). Percobaan ini dapat anda skip jika anda telah yakin bahwa backend yang anda buat sudah berfungsi dengan baik.

### Percobaan 6

Pada percobaan ini kita akan membuat interface utama untuk program kita yaitu GUI.

Lakukan hal yang sama untuk data **Anggota**!

### Percobaan 7

Buat form untuk data Anggota.

Untuk data **Buku**, caranya kurang lebih sama seperti data Kategori dan Anggota. Hanya saja yang
berbeda adalah:

* Pemanggilan **getKategori().getIdKategori()** pada query insert dan update untuk mengeset **idkategori** pada tabel buku
* Query select yang melibatkan join table.

Kode lengkap class Buku dapat anda lihat di **Lampiran 1**. Untuk test buku pada **frontend**, bisa anda lihat di **Lampiran 2**.

### Percobaan 8

Membuat GUI untuk data Buku, yang dilengkapi dengan combo box untuk memilih kategori, yang terhubung dengan tabel kategori.

## Tugas

1. Buatlah class **Peminjaman**.
2. Buatlah class **FrmPeminjaman** dan susun sebagai berikut:

    ![Soal tugas2](img/tugas2-soal.png)

3. Atur kode program agar dapat menangani transaksi peminjaman dan pengembalian

## Kesimpulan

1. Saya mampu menggunakan paradigma berorientasi objek untuk interaksi dengan database.
2. Saya mampu membuat backend dan frontend.
3. Saya mampu membuat form sebagai frontend.

## Pernyataan Diri

Saya menyatakan isi tugas, kode program, dan laporan praktikum ini dibuat oleh saya sendiri. Saya tidak melakukan plagiasi, kecurangan, menyalin/menggandakan milik orang lain.

Jika saya melakukan plagiasi, kecurangan, atau melanggar hak kekayaan intelektual, saya siap untuk mendapat sanksi atau hukuman sesuai peraturan perundang-undangan yang berlaku.

Ttd,

***Sultan Achmad Qum Masykuro NS***
