# Lab7Web - Pratikum PHP Dasar

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI 24 A4

Matakuliah: Pemograman Web 1

# Deskripsi

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



