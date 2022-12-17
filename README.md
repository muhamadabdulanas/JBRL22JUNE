# praktikum9

## Exception Handling
#### . Exception (eksepsi) merupakan suatu kesalahan (error) yang terjadi saat proses eksekusi program sedang berjalan,
#### .Kesalahan ini akan menyebabkan program berakhir dengan tidak normal.
## Handling
#### Penanganan file adalah bagian penting dari aplikasi apa pun.
## Assertion
#### Assertion(pernyataan) adalah kewajaran program yang kamu bisa aktif/nonaktifkan ketika kamu selesai menjalankan program.
## The Assert Statement
#### Saat menemukan pernyataan, Python mengevaluasi ekspresi yang menyertainya, yang mana semoga benar. Jika ekspresi salah, Python memunculkan pengecualian AssertionError.
### Sintaks untuk pernyataan yaitu :
assert Expression[, Arguments]
#### jika pernyataan gagal, Python menggunakan ArgumentExpression ArgumentExpression sebagai argumen argumen untuk AssertionError AssertionError. Pengecualian AssertionError Pengecualian AssertionError dapat ditangkap dan ditangani ditangani seperti pengecualian lainnya menggunakan try- kecuali pernyataan, tetapi jika dibiarkan, mereka akan menghentikan program dan menghasilkan backtrace
### Contoh
#### Berikut adalah fungsi fungsi yang mengubah suhu dari derajat Kelvin menjadi derajat Fahrenheit.Karena nol derajat Kelvin dingin, fungsi fungsi menyimpannya jika melihat negatif negatif suhu.
#### Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![9 1](https://user-images.githubusercontent.com/115569493/208219641-c88075f8-9dfd-4576-9965-1b0d754bcfbd.png)

## Menangani Pengecualian
#### jika Anda memiliki beberapa kode mencurigakan yang mungkin mengeluarkan pengecualian, Anda dapat mempertahankan program Anda letakkan kode yang mencurigakan di try: blok. Setelah coba: blok, sertakan pernyataan sertakan except: statemen, diikuti oleh blok kode yang menangani masalah seanggun mungkin.

### Contoh
#### Contoh-contoh ini membuka file, menulis konten file, dan keluar dengan aman karena ada tidak masalah
#### Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:!

[9 2](https://user-images.githubusercontent.com/115569493/208219753-a6138581-293a-40fa-89c3-11e467ab7aeb.png)

#### Contoh ini mencoba membuka file yang Anda tidak memiliki izin menulis, sehingga membuat file pengecualian
#### Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![9 3](https://user-images.githubusercontent.com/115569493/208219806-50daf461-61e4-4c4b-89c2-536fa41b8120.png)

## Fasal kecuali tanpa Pengecualian
#### Anda juga dapat menggunakan pernyataan exception tanpa exception yang didefinisikan sebagai berikut:

##### try:
##### You do your operations here;
##### ......................
##### except:
##### If there is any exception, then execute this block.
##### ......................
##### else:
##### If there is no exception then execute this block.
#### Pernyataan coba-kecuali jenis ini menangkap semua pengecualian pengecualian yang terjadi. Menggunakan percobaan seperti try-expect pernyataan tidak dianggap sebagai praktik pemrograman yang baik, karena mereka menangkap semuanya pengecualian tetapi tidak membuat programmer mengidentifikasi kemungkinan penyebab masalah terjadi

### Klausa kecuali dengan Berbagai Pengecualian
#### Anda juga dapat menggunakan pernyataan exception yang sama untuk menangani beberapa exception sebagai berikut:
##### try:
##### You do your operations here;
##### ......................
##### except(Exception1[, Exception2[,...ExceptionN]]]):
##### If there is any exception from the given exception list,
##### then execute this block.
##### ......................
##### else:
##### If there is no exception then execute this block.

## Klausa coba-akhirnya
### Contoh
#### Jika Anda tidak memiliki izin untuk membuka file dalam mode tulis yang dapat ditulis, maka ini akan menghasilkan hasil berikut

![207681346-73508e3b-a892-4b29-9ca8-77d3d1ef3916](https://user-images.githubusercontent.com/115569493/208220004-0ab186a8-62b9-4347-880e-5f233d67dd1b.png)

Contoh yang sama dapat ditulis lebih bersih sebagai berikut:

![9 4](https://user-images.githubusercontent.com/115569493/208220031-1832ed66-d8d2-4f16-a7e9-d938c38b0c65.png)

Ketika exception dilempar ke dalam blok try, eksekusi segera dilanjutkan ke akhir memblok. Setelah semua pernyataan di blok akhirnya dieksekusi, pengecualian dimunculkan lagi dan ditangani dalam pernyataan kecuali jika ada di lapisan berikutnya yang lebih tinggi dari percobaan-kecuali penyataan.

## Argumen Pengecualian
### Contoh
#### Berikut adalah contoh untuk satu pengecualian
#### Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:

![9 5](https://user-images.githubusercontent.com/115569493/208220084-f7651e3b-ede0-4ad7-b5ff-e25430262d09.png)

## Melempar Pengecualian
### Contoh
#### Pengecualian dapat berupa string, kelas, atau objek. Sebagian besar pengecualian adalah pengecualian dari inti Python menimbulkan adalah kelas, dengan argumen=argumen yang merupakan turunan dari kelas. Mendefinisikan pengecualian barucukup mudah dan dapat dilakukan sebagai berikut:

![9 6](https://user-images.githubusercontent.com/115569493/208220305-53b9dc61-cfb6-49da-adcb-85738f0f8bc6.png)

## Pengecualian yang Ditetapkan Pengguna
#### Python juga memungkinkan Anda membuat pengecualian sendiri dengan menurunkan kelas-kelas dari yang standar pengecualian bawaan.
#### Berikut adalah contoh-contoh yang terkait dengan RuntimeError. Di sini, kelas dibuat yang merupakan subkelas dari subkelas RuntimeError. Ini berguna saat Anda perlumenampilkan tampilan informasi yang lebih spesifik saat e pengecualian tertangkap.
#### Di blok coba, pengecualian yang ditentukan pengguna dimunculkan dan ditangkap di blok kecuali. Itu variabel e digunakan untuk membuat instance dari kelas Networkerror.

![9 7](https://user-images.githubusercontent.com/115569493/208220344-e6384817-e391-4327-b63d-18116ecf8237.png)



