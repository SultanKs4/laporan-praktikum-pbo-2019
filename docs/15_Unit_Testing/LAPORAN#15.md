# Laporan Praktikum #15 - Unit Testing

## Kompetensi

1. Memahami konsep dan fungsi unit testing
2. Menerapkan unit testing dengan JUnit pada program sederhana.
3. Menerapkan unit testing dengan JUnit pada progam yang terkoneksi database

## Ringkasan Materi

Unit testing adalah sebuah kode yang ditulis oleh developer, yang digunakan untuk menguji bagian kecil/area spesifik dari suatu aplikasi yang telah/sedang dibuat. Unit testing bertujuan untuk menghilangkan kebutuhan akan pengujian manual kode aplikasi oleh manusia (tester/QC). Sehingga dengan kata lain unit testing adalah usaha untuk mengotomatiskan pengujian kode program (automated test) Kode tes tidak akan dikirimkan ke user, melainkan hanya production code (kode yang digunakan dalam program utama) saja yang dikirim. Unit testing dilakukan setelah programmer selesai menuliskan suatu kode/fungsi/method yang ada dalam suatu class. Dapat juga dilakukan setelah menambahkan sebuah fungsionalitas baru atau setelah melakukan refactoring.

### JUnit

JUnit adalah sebuah framework unit testing untuk bahasa Java yang bersifat open source yang dapat digunakan untuk menulis dan menjalankan software testing secara berulang-ulang. JUnit mengikuti arsitektur xUnit dalam pembuatannya. JUnit
dikembangkan oleh Erich Gamma dan Kent Beck. JUnit dapat diperoleh dengan mengunduhnya dari situs [disini](http://junit.sourceforge.net/).

Permasalahan utama yang sering muncul pada pengujian dengan metode konvensional adalah tidak efisiennya penggunaan waktu. Menuliskan statement- statement debug ke dalam kode adalah metode yang kurang efektif. Metode ini mengharuskan developer untuk mengamati output program dengan cermat setiap kali program dijalankan untuk memastikan program berjalan dengan benar. Dengan menggunakan JUnit untuk mengkodekan ekspektasi-ekspektasi dalam bentuk Automated Unit Testing, maka kegiatan pengujian menjadi lebih singkat.

Dalam unit testing, terdapat beberapa aturan penamaan yang harus diikuti. Sebuah test class harus memiliki nama yang sama dengan class yang akan di-test dan diberiprefix “test”. Contoh: Sebuah class Account akan memiliki sebuah test class dengan nama TestAccount.

Penamaan tersebut dimaksudkan untuk mempermudah dalam mengorganisasi unit testing. Sebuah test class harus merupakan turunan (extends) dari class `junit.framework.TestCase.` Untuk dapat menggunakan semua fungsi yang ada dalam package JUnit, kita harus meng-importjunit.framework.* pada tiap test class yang akan kita tulis.

`Test Runner` yang digunakan mempunyai fitur untuk mencari sekumpulan test case dalam suatu test class. Agar fitur tersebut dapat berfungsi, kita harus mendefinisikan method TestSuite(), yang mengembalikan instance TestCase atau TestSuite. Keduanya merupakan implementasi dari interface class Test. Test Suite juga dapat digunakan untuk mengeksekusi test method, dimana nama test method tersebut tidak menggunakan kata “test”.

`Method assert` adalah suatu method yang akan membantu dalam menentukan sebuah method yang sedang ditest/diuji berjalan dengan baik atau tidak. Bila sebuah method mengalami kegagalan, eksekusi dari test method tersebut akan dibatalkan sedangkan test untuk method yang lainnya akan tetap berjalan.

## Percobaan

### Percobaan 1

Pada percobaan yang pertama ini kita akan membuat sebuah program sederhana yang mengilustrasikan sebuah aplikasi pengiriman pesan. Pada program tersebut terdapat satu class utama dimana didalamnya terdapat beberapa method sederhana yang nantinya akan dibuatkan unit test-nya.

`Screenshot`

![Percobaan 1 SS](img/percobaan1-ss.png)

![Percobaan 1 SS 2](img/percobaan1-ss2.png)

`Kode Program`

* [MessageProcessor1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/unittest/MessageProcessor1841720019Sultan.java)
* [LearnUnitTesting1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/unittest/LearnUnitTesting1841720019Sultan.java)
* [MessageProcessor1841720019SultanTest.java](../../src/15_Unit_Testing/test/java/id/natlus/jobsheet15/unittest/MessageProcessor1841720019SultanTest.java)
* [TestRunner1841720019Sultan.java](../../src/15_Unit_Testing/test/java/id/natlus/jobsheet15/unittest/TestRunner1841720019Sultan.java)

### Percobaan 2

Pada percobaan kedua kita akan mencoba membuat test case dari salah satu percobaan pada jobsheet minggu ke 14. Struktur file dari percobaan ke satu terdiri dari 4 file class yaitu DBHelper.java, FormKategori.java, Kategori.java dan TestBackend.java.

`Screenshot`

![Percobaan 2 SS](img/percobaan2-ss.png)

![Percobaan 2 SS 2](img/percobaan2-ss2.png)

`Kode Progam`

* [Kategori1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/backend/Kategori1841720019Sultan.java)
* [DBHelper1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/backend/DBHelper1841720019Sultan.java)
* [TestBackend1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/frontend/TestBackend1841720019Sultan.java)
* [FrmKategori1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/frontend/FrmKategori1841720019Sultan.java)
* [FrmKategori1841720019Sultan.form](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/frontend/FrmKategori1841720019Sultan.form)
* [Kategori1841720019SultanTest.java](../../src/15_Unit_Testing/test/java/id/natlus/jobsheet15/database/backend/Kategori1841720019SultanTest.java)
* [TestRunner1841720019Sultan.java](../../src/15_Unit_Testing/test/java/id/natlus/jobsheet15/unittest/TestRunner1841720019Sultan.java)

## Tugas

1. Buat test case untuk percobaan kedua pada jobsheet ke 14

`Screenshot`

![tugas 1 ss](img/tugas-ss.png)
![tugas 1 ss 2](img/tugas-ss2.png)

`Kode Program`

* [Anggota1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/backend/Anggota1841720019Sultan.java)
* [DBHelper1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/backend/DBHelper1841720019Sultan.java)
* [TestBackendAnggota1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/frontend/TestBackendAnggota1841720019Sultan.java)
* [FrmAnggota1841720019Sultan.java](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/frontend/FrmAnggota1841720019Sultan.java)
* [FrmAnggota1841720019Sultan.form](../../src/15_Unit_Testing/main/java/id/natlus/jobsheet15/database/frontend/FrmAnggota1841720019Sultan.form)
* [Anggota1841720019SultanTest.java](../../src/15_Unit_Testing/test/java/id/natlus/jobsheet15/database/backend/Anggota1841720019SultanTest.java)
* [TestRunner1841720019Sultan.java](../../src/15_Unit_Testing/test/java/id/natlus/jobsheet15/unittest/TestRunner1841720019Sultan.java)

## Kesimpulan

1. Saya mampu memahami konsep dan fungsi unit testing
2. Saya mampu menerapkan unit testing dengan JUnit pada program sederhana.
3. Saya mampu menerapkan unit testing dengan JUnit pada progam yang terkoneksi database

## Pernyataan Diri

Saya menyatakan isi tugas, kode program, dan laporan praktikum ini dibuat oleh saya sendiri. Saya tidak melakukan plagiasi, kecurangan, menyalin/menggandakan milik orang lain.

Jika saya melakukan plagiasi, kecurangan, atau melanggar hak kekayaan intelektual, saya siap untuk mendapat sanksi atau hukuman sesuai peraturan perundang-undangan yang berlaku.

Ttd,

***Sultan Achmad Qum Masykuro NS***
