# lab5web
# Nama      : Muhammad Albedri
# NIM       : 312210290
# Kelas     : TI 22 A3

# Praktikum5
# Instruksi Praktikum
* 1. Persiapkan text editor misalnya VSCode.
* 2. Buat folder baru dengan nama lab5_javascript.
* 3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
* 4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org
# Langkah-langkah Praktikum
* Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Mengenal JavaScript</title>
    </head>
    <body>
        <h1>Pengenalan JavaScript</h1>
        <h3>Contoh dokument.write dan console.log</h3>
        <script>
            document.write("Hello World");
            console.log("Hello World");
        </script>
    </body>
</html>

```
![gambar1](/lab5_js/img/output%201.png)

# Javascrip Dasar
* Pemakaian Alert sebagai property window.
```
<html>
    <head>
        <title>alert box</title>
    </head>
    <body>
        <script language = "JavaScript">
            <!--
                window.alert("ini merupakan pesan untuk anda");
            //-->
        </script>
    </body>
</html>
```
![gambar2](/lab5_js/img/output%202.png)

* Pemakaian method dalam objek
```
<html>
    <head>
        <title>skrip JavaScript</title>
    </head>
    <body>
        percobaan memakai JavaScript:<br>
        <script language = "JavaScript">
            <!--
                document.write("selamat mencoba javascript");
                document.write("semoga sukses!");
            //-->
        </script>
    </body>
</html>
```
![gambar3](/lab5_js/img/output%203.png)

* Pemakaian method dalam objek
```
<html>
    <head>
        <title>pemasukan data</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                var nama = prompt("siapa nama anda?","masukan nama anda");
                document.write("hai,"+ nama);
            //-->
        </script>
    </body>
</html>
```
![gambar4.0](/lab5_js/img/output%204.0.png)
![gambar4.1](/lab5_js/img/output%204.1.png)

* Pembuatan fungsi dan cara pemanggilannya
```
<html>
    <head>
        <title>contoh program javascript</title>
        <script language = "javascript">
            function pesan(){
                alert ("memanggil javascript lewat body onload")
            }
        </script>
    </head>
    <body onload = pesan()>
    </body>
</html>
```
![gambar5](/lab5_js/img/output%205.png)

# Dasar Pemrograman Di Javascript
* Operasi dasar aritmatika
```
<html>
    <head>
        <title>contoh program javascript</title>

        <script language = "javascript">
            function test (val1,val2)
            {
                document.write("<br>"+"perkalian : val1*val2 "+"<br>")
                document.write(val1*val2)
                document.write("<br>"+"pembagian : val1/val2 "+"<br>")
                document.write(val1/val2)
                document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
                document.write(val1+val2)
                document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
                document.write(val1-val2)
                document.write("<br>"+"modulus : val1%val2 "+"<br>")
                document.write(val1%val2)
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="arithmatic" onclick="test(9,4)">
    </body>
</html>
```
![gambar6](/lab5_js/img/output%206.png)

* Seleksi kondisi (if..else)
```
<html>
    <head>
        <title>contoh if-else</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                var nilai = prompt("nilai (0-100): ",0);
                var hasil = "";
                if (nilai >= 60)
                hasil = "lulus";
                else
                hasil = "tidak lulus";
                document.write("hasil: " + hasil);
            //-->
        </script>
    </body>
</html>
```
![gambar7.0](/lab5_js/img/output%207.0.png)
![gambar7.1](/lab5_js/img/output%207.1.png)

* Penggunaan operator switch untuk seleksi kondisi
```
<html>
    <head>
        <title>contoh program javascript</title>

        <script language = "javascript">
            function test ()
            {
                val1=window.prompt ("input nilai (1-5):")
                switch (val1)
                {
                    case "1" :
                        document.write("bilangan satu")
                        break
                    case "2" :
                        document.write("bilangan dua")
                        break
                    case "3" :
                        document.write("bilangan tiga")
                        break
                    case "4" :
                        document.write("bilangan empat")
                        break
                    case "5" :
                        document.write("bilangan lima")
                        break
                    default :
                        document.write("bilangan lainnya")
                }
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="switch" onclick=test()>
    </body>
</html>
```
![gambar8.0](/lab5_js/img/output%208.0.png)
![gambra8.1](/lab5_js/img/output%208.1.png)

# Pembuatan Form
* Form Input
```
<html>
    <head>
        <script language = "javascript">
            function test () {
                var val1=document.kirim.T1.value
                if (val1%2==0)
                    document.kirim.T2.value="bilangan genap"
                else
                    document.kirim.T2.value="bilangan ganjil"
            }
            </script>
    </head>
    <body>
        <form method="post" name="kirim">
            <p>BIL <input type="text" name="T1" size="20">
            MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
            <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
        </form>
    </body>
</html>
```
![gambar9](/lab5_js/img/output%209.png)

* Form Button
```
<html>
    <head>
        <title>objek document</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                function ubahWarnaLB(warna) {
                    document.bgColor = warna;
                }
                function ubahWarnaLD(warna) {
                    document.fgColor = warna
                }
            //-->
        </script>

        <h1>tes</h1>
        <form>
            <input type="button" value="latar belakang hijau" onclick="ubahWarnaLB('GREEN')">
            <input type="button" value="latar belakang putih" onclick="ubahWarnaLB('WHITE')">
            <input type="button" value="test kuning" onclick="ubahWarnaLD('YELLOW')">
            <input type="button" value="test biru" onclick="ubahWarnaLD('BLUE')">
        </form>
        <script language = "javascript">
            <!--
                document.write("Dimodifikasi terakhir pada" +
                document.LastModified);    
            //-->
        </script>
    </body>
</html>
```
![gambar10](/lab5_js/img/output%2010.png)

# HTML DOM
* Pilihan menggunakan checkBox dengan perhitungan otomatis
```
<!--
    file: daftar_menu.html    
//-->
<html>
    <head>
        <title>daftar Menu</title>
        <script>
            function hitung(ele) {
                var total = document.getElementByid('total').value;
                    total = (total ? parseiInt(total) : 0);
                var harga = 0;

                if (ele.checked) {
                    harga = ele.value;
                    total += perseInt(harga);
                } else {
                    harga = ele.value;
                    if (total > 0)
                        total = perseInt(harga);
                }

                document.getElementByid('total').value = total;
            }
        </script>
    </head>
    <body>
        <h1>Daftar Menu Makanan</h1>
        <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this)" /> Ayam Goreng Rp. 5.000</label><br />
        <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this)" /> Tmpe Goreng Rp. 500</label><br />
        <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this)" /> Telur Dadar Rp. 2.500</label><br />
        <strong>Total Bayar: Rp. <input id="total" type="text" /> </strong>
    </body>
</html>
```
![gambar11](/lab5_js/img/output%2011.png)

# Pertanyaan dan Tugas
* 1. Buat script untuk melakukan validasi pada isian form.
# Laporan Praktikum
* 1. Buatlah repository baru dengan nama Lab5Web.
* 2. Kerjakan semua latihan yang diberikan sesuai urutannya.
* 3. Screenshot setiap perubahannya.
* 4. Buatlah file README.md dan tuliskan penjelasan dari setiap langkah praktikum beserta screenshotnya.
* 5. Commit hasilnya pada repository masing-masing.
* 6. Kirim URL repository pada e-learning ecampus