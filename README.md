# Lab7Web - Pratikum PHP Dasar

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI 24 A4

Matakuliah: Pemograman Web 1

# PHP Dasar

<img width="950" height="475" alt="Screenshot 2025-11-17 102920" src="https://github.com/user-attachments/assets/4b512e51-ed59-4eb2-8c1b-21a105e8f9f8" />

```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World";
    ?>
</body>
</html>
```


<img width="1224" height="522" alt="Screenshot 2025-11-17 104206" src="https://github.com/user-attachments/assets/d384366c-ead2-40af-841d-eead4390f295" />


Kode tersebut adalah sebuah halaman web sederhana yang menggunakan HTML dan PHP. Bagian paling atas `<!DOCTYPE html>` menunjukkan bahwa dokumen ini adalah HTML5. Lalu pada tag `<html lang="id">`, halaman diatur agar menggunakan bahasa Indonesia. Di dalam bagian `<head>`, terdapat `<meta charset="UTF-8">` yang berfungsi menentukan karakter encoding agar teks yang muncul dapat ditampilkan dengan benar, dan `<title>PHP Dasar</title>` yang akan tampil sebagai judul tab di browser.

Selanjutnya, bagian `<body>` adalah area yang tampil pada layar. Di sana terdapat tulisan “Belajar PHP Dasar” yang dibuat menggunakan tag `<h1>` sehingga tampil sebagai judul besar. Setelah itu terdapat bagian PHP yang ditandai dengan `<?php ... ?>`. Di dalamnya ada perintah `echo "Hello World";` yang digunakan untuk menampilkan teks ke halaman web. Jadi ketika file ini dijalankan di server yang mendukung PHP, halaman akan menampilkan judul “Belajar PHP Dasar” diikuti teks “Hello World”. Kode ini merupakan bentuk paling dasar dari kombinasi HTML dan PHP untuk menampilkan output pertama.

# Variable PHP

# Predefine PHP

<img width="956" height="533" alt="image" src="https://github.com/user-attachments/assets/25dccad2-b63a-4abf-b11c-d06fe246e8d0" />


# From Input

<img width="952" height="602" alt="image" src="https://github.com/user-attachments/assets/127921c2-2730-4314-8f56-af6f7ad305f7" />




# Tugas LAB7WEB

Program ini merupakan aplikasi PHP dasar yang memanfaatkan sebuah media input data. Pengguna dapat memasukkan **nama**, **tanggal lahir**, serta **jenis pekerjaan** yang dipilih dari daftar pilihan.

Setelah data dikirimkan, PHP akan memprosesnya dengan cara:

- Menghitung usia pengguna secara otomatis berdasarkan tanggal lahir yang diberikan.
-  Menentukan besaran gaji sesuai pekerjaan yang dipilih, menggunakan struktur kontrol **switch-case** untuk membedakan setiap kategori pekerjaan.
- Menampilkan kembali seluruh hasil input beserta perhitungan pada halaman yang sama.

Program ini mempelajari cara kerja form, pengolahan data, dan pengambilan keputusan dalam PHP.

# Langkah - Langkah

1. **Membuat Form Input**

   * Buat sebuah halaman PHP yang berisi form menggunakan tag `<form>`.
   * Tambahkan input untuk **nama** menggunakan `<input type="text">`.
   * Tambahkan input untuk **tanggal lahir** menggunakan `<input type="date">`.
   * Sediakan pilihan pekerjaan menggunakan `<select>` beserta beberapa `<option>`.

2. **Mengambil Data Menggunakan Metode POST**

   * Atur atribut `method="POST"` pada form.
   * Tangkap data yang dikirim form menggunakan `$_POST['nama']`, `$_POST['tanggal']`, dan `$_POST['pekerjaan']`.

3. **Menghitung Umur dari Tanggal Lahir**

   * Ubah tanggal lahir menjadi objek `DateTime`.
   * Gunakan fungsi `date_diff()` antara tanggal lahir dan tanggal hari ini.
   * Ambil hasil umur dalam satuan tahun.

4. **Menentukan Gaji Berdasarkan Pekerjaan**

   * Buat struktur `switch` yang memeriksa nilai dari pekerjaan.
   * Setiap case berisi jumlah gaji tertentu.
   * Tambahkan `default` jika tidak ada pekerjaan yang sesuai.

5. **Menampilkan Output di Halaman yang Sama**

   * Setelah tombol submit ditekan, tampilkan hasil:

     * Nama
     * Usia
     * Pekerjaan
     * Gaji yang ditentukan oleh `switch`
   * Tampilkan hasil di bawah form pada file yang sama.

6. **Melakukan Commit ke Repository GitHub**

   * Buka folder project menggunakan Git Bash atau terminal.
   * Jalankan perintah:

     - `git add .`
     - `git commit -m "Menambahkan program PHP form input dan perhitungan"`
     -  `git push`
   * Pastikan repository GitHub sudah dibuat dan remote sudah terhubung.


# 📷 Hasil Screenshot (Tampilan Code)

# 📃 Hasil Output Program



