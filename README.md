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

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>

    <?php
    // Menampilkan teks Hello World
    echo "Hello World<br>";

    // Menampilkan subjudul di bawah Hello World
    echo "<h2>Menggunakan Variabel</h2>";

    // Deklarasi variabel
    $nim = "312410338";
    $nama = "Marsya Nabila";

    // Menampilkan isi variabel
    echo "NIM : " . $nim . "<br>";
    echo "Nama : " . $nama;
    ?>
</body>
</html>
```

<img width="949" height="661" alt="image" src="https://github.com/user-attachments/assets/3382b6d3-46fe-433f-90ac-57b57f3d183a" />

Kode tersebut membuat halaman web sederhana yang menampilkan teks menggunakan PHP. Pada bagian HTML ditampilkan judul “Belajar PHP Dasar”. Di dalam tag PHP, pertama-tama kode menampilkan tulisan “Hello World”. Setelah itu ditampilkan subjudul “Menggunakan Variabel”. Dua variabel dibuat, yaitu `$nim` berisi “312410338” dan `$nama` berisi “Marsya Nabila”. Kedua variabel ini kemudian ditampilkan ke halaman menggunakan `echo`, sehingga muncul teks NIM dan Nama sesuai isi variabel tersebut.



# Predefine PHP

```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Predefine Variable</title>
</head>
<body>
    <h1>Predefine Variable</h1>

    <?php
    if (isset($_GET['nama'])) {
        echo 'Selamat Datang ' . $_GET['nama'];
    } else {
        echo 'Selamat Datang, Marsya Nabila!';
    }
    ?>
</body>
</html>
```


<img width="956" height="533" alt="image" src="https://github.com/user-attachments/assets/25dccad2-b63a-4abf-b11c-d06fe246e8d0" />

Kode tersebut membuat halaman web yang menampilkan sambutan menggunakan variabel bawaan PHP. Bagian HTML hanya menampilkan judul “Predefine Variable”. Pada bagian PHP, program mengecek apakah di URL terdapat data `nama` melalui `$_GET['nama']`. Jika ada, maka halaman akan menampilkan “Selamat Datang” diikuti nama yang dikirim lewat URL. Jika tidak ada data tersebut, maka akan muncul sambutan default yaitu “Selamat Datang, Marsya Nabila!”. Dengan kata lain, halaman ini menampilkan nama sesuai input dari URL, tetapi tetap punya nama bawaan kalau tidak ada input.


# From Input
```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Form Input</title>
</head>
<body>
    <h2>Form Input</h2>

    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>

    <?php
    // Menampilkan teks di bawah form
    echo 'Selamat Datang Marsya Nabila';
    ?>
</body>
</html>
```


<img width="952" height="602" alt="image" src="https://github.com/user-attachments/assets/127921c2-2730-4314-8f56-af6f7ad305f7" />

Kode tersebut membuat sebuah halaman yang menampilkan form sederhana untuk memasukkan nama. Form menggunakan metode POST dan memiliki satu input teks serta tombol Kirim. Namun, meskipun ada form, nilai dari input tidak diproses; bagian PHP di bawahnya hanya menampilkan teks tetap yaitu “Selamat Datang Marsya Nabila”. Jadi apa pun yang diisi di form tidak memengaruhi output, karena program tidak mengambil data dari form dan hanya menampilkan sambutan statis.


# Operator 
```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Operator PHP</title>
</head>
<body>
    <h2>Operator Aritmatika di PHP</h2>
    <?php
        $gaji = 1000000;
        $pajak = 0.1;
        $thp = $gaji - ($gaji * $pajak);

        echo "Gaji sebelum pajak = Rp. $gaji <br>";
        echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
</body>
</html>
```

<img width="949" height="475" alt="image" src="https://github.com/user-attachments/assets/5585c3cd-7b68-4f3d-97ab-b4bf78acfa37" />

Kode tersebut menghitung gaji bersih menggunakan operator aritmatika di PHP. Variabel `$gaji` berisi 1.000.000 dan `$pajak` berisi 0.1 (artinya 10%). Kemudian `$thp` dihitung dari gaji dikurangi hasil perkalian gaji dengan pajak. Setelah perhitungan selesai, program menampilkan gaji sebelum pajak dan gaji yang dibawa pulang. Hasilnya adalah tampilan dua baris yang menunjukkan nilai gaji awal dan gaji setelah dipotong pajak.


# Kondisi
```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Struktur Kondisi PHP</title>
</head>
<body>
    <h2>Struktur Kondisi IF dan SWITCH</h2>
<?php
$nama_hari = date("l");
if ($nama_hari == "Sunday") {
    echo "Minggu";
} elseif ($nama_hari == "Monday") {
    echo "Senin";
} else {
    echo "Hari ini bukan Minggu atau Senin";
}

echo "<hr>";

switch ($nama_hari) {
    case "Sunday":
        echo "Minggu";
        break;
    case "Monday":
        echo "Senin";
        break;
    case "Tuesday":
        echo "Selasa";
        break;
    default:
        echo "Hari lainnya";
}
?>
```


<img width="945" height="588" alt="image" src="https://github.com/user-attachments/assets/dcde92da-93fa-495b-959d-a66fd988c70d" />

Kode tersebut menampilkan nama hari menggunakan dua jenis struktur kondisi, yaitu **IF** dan **SWITCH**. Variabel `$nama_hari` mengambil nama hari sekarang dalam bahasa Inggris lewat `date("l")`. Bagian IF mengecek apakah hari itu Sunday atau Monday; jika Sunday ditampilkan “Minggu”, jika Monday ditampilkan “Senin”, dan selain itu ditampilkan pesan bahwa hari ini bukan kedua hari tersebut. Setelah garis pemisah `<hr>`, bagian SWITCH melakukan pengecekan yang sama tetapi dengan lebih banyak pilihan, yaitu Sunday, Monday, dan Tuesday. Jika tidak masuk salah satu dari ketiganya, maka akan tampil “Hari lainnya”. Dengan begitu, kode ini menunjukkan dua cara berbeda untuk mengecek kondisi berdasarkan nama hari.


# Perulangan

## 1. for

```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Perulangan for</title>
</head>
<body>
    <h2>Perulangan for (1 sampai 10)</h2>

    <?php
        for ($i = 1; $i <= 10; $i++) {
            echo "Perulangan ke-$i<br>";
        }

        echo "<hr>";

        echo "Perulangan menurun dari 10 ke 1<br>";
        for ($i = 10; $i >= 1; $i--) {
            echo "Perulangan ke-$i<br>";
        }
    ?>
</body>
</html>
```

<img width="953" height="759" alt="image" src="https://github.com/user-attachments/assets/f5c6c67c-e478-42ba-84e8-e684035a496f" />

Kode tersebut menampilkan dua jenis perulangan menggunakan **for**. Perulangan pertama berjalan dari angka 1 sampai 10, sehingga setiap putaran mencetak teks “Perulangan ke-” diikuti nomor urutnya. Setelah itu dibuat garis pemisah `<hr>`. Lalu perulangan kedua berjalan dari angka 10 turun ke 1, sehingga hasilnya menampilkan urutan menurun. Dengan kata lain, kode ini menunjukkan contoh loop naik dan loop turun menggunakan struktur for di PHP.


## While

```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Perulangan while</title>
</head>
<body>
    <h2>Perulangan while (1 sampai 10)</h2>

    <?php
        $i = 1;
        while ($i <= 10) {
            echo "Perulangan ke-$i<br>";
            $i++;
        }
    ?>
</body>
</html>
```

<img width="958" height="667" alt="image" src="https://github.com/user-attachments/assets/bd55799f-baea-4679-a02b-0a23f6a176e7" />

Kode tersebut menampilkan perulangan menggunakan **while**. Variabel `$i` mulai dari 1, lalu selama nilainya masih kurang atau sama dengan 10, perulangan akan terus berjalan. Di dalam loop, program mencetak teks “Perulangan ke-” sesuai nilai `$i`, kemudian `$i` ditambah satu setiap putaran. Hasilnya, halaman menampilkan urutan dari 1 sampai 10 menggunakan struktur while.



## DO While

```
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Perulangan do...while</title>
</head>
<body>
    <h2>Perulangan do...while (1 sampai 10)</h2>

    <?php
        $i = 1;
        do {
            echo "Perulangan ke-$i<br>";
            $i++;
        } while ($i <= 10);
    ?>
</body>
</html>
```


<img width="940" height="572" alt="image" src="https://github.com/user-attachments/assets/256ffe28-7b13-4688-8ffe-a0a5fa9114ec" />

Kode tersebut menampilkan perulangan menggunakan **do...while**. Nilai `$i` dimulai dari 1, lalu bagian `do` akan dijalankan terlebih dahulu untuk menampilkan teks “Perulangan ke-” beserta angkanya. Setelah itu `$i` ditambah satu, kemudian kondisi `while ($i <= 10)` dicek. Selama kondisi masih benar, perulangan akan terus diulang. Karena bagian `do` selalu dijalankan minimal sekali, urutan angka 1 sampai 10 akan tampil pada halaman.









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

<img width="1388" height="2838" alt="1111" src="https://github.com/user-attachments/assets/905062a6-9905-497a-9010-8a82a54d577e" />


# 📃 Hasil Output Program

<img width="957" height="774" alt="image" src="https://github.com/user-attachments/assets/f16188b8-5c05-41a8-84f6-2a7ee441b1c5" />




