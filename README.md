# Modul7PHP
1. Berikan contoh kode keneksi untuk ke database pd php?
    $connect = mysqli_connect($host, $uname, $pass, $db);

2. Bagaimana cara anda membuat database pada phpMySQl!
    <?php
        include '../connect.php';
        $nama_dosen = $_POST['nama_dosen'];
        $telp = $_POST['telp'];
        $query = "INSERT INTO dosen(nama_dosen, telp) VALUES ('$nama_dosen','$telp')";
        $result = mysqli_query($connect,$query);
        $num = mysqli_affected_rows($connect);
        if ($num > 0) {
          echo "Berhasil tambah data";
        } else {
          echo "Gagal tambah data";
        }
        echo "<a href='read.php'>Lihat Data</a>";
            ?>

3. Berikan code query untuk menampilkan sebuah data yang ada pada ke database?
    SELECT * FROM dosen

4. Berikan code query untuk mengupdate sebuah data yang ada pada ke database?
    UPDATE nama_tabel SET nama_kolom = data_baru WHERE kondisi
    UPDATE dosen SET nama_dosen = '$nama_dosen', telp = '$telp' WHERE id_dosen

5. Berikan code query untuk menghapus sebuah data yang ada pada ke database?
    DELETE FROM nama_tabel WHERE kondisi
    DELETE FROM dosen WHERE id_dosen

# HASIL
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/11.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/12.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/13.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/14.PNG)

![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/21.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/22.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/23.PNG)

![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/31.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/32.PNG)
![alt text](https://github.com/rashadandredi/Modul7PHP/blob/master/hasil/33.PNG)
