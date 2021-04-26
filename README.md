# Praktikum 5 - Pemrograman Web
```
Ajisahraji
311910335
TI.19.A.2
Universitas Pelita Bangsa
```
## buat dokumen HTML dengan nama file lab5_javascript.html dan masukan coding
![LANGKAH 1 membuat javascript]

# Java Script Dasar
## Pemakaian Alert sebagai property window
![LANGKAH 2 membuat alert box]
## Pemakaian method dalam objek
![LANGKAH 3 Pemakaian metod]
## Pemakaian Prompt
![LANGKAH 4 Pemakaian prompt]
## Pembuatan fungsi dan cara pemanggilannya
![LANGKAH 5 Pembuatan fungsi dan pemanggilan]

# Dasar Pemrograman Di Javascript
## Operasi dasar Aritmatika
![LANGKAH 6 Operasi dasar Aritmatika]

## Seleksi kondisi (if..else)
* Coding
![LANGKAH 7 seleksi kondisi (coding)]

* Output

![LANGKAH 7 seleksi kondisi (hasil 1)]

![LANGKAH 7 seleksi kondisi (hasil 2)]

## Penggunaan operator switch untuk seleksi kondisi
* Coding
![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (coding)]
* Output

![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (hasil 1)]
![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (hasil 2)]

# Pembuatan Form
## Form Input
* Coding
![LANGKAH 9 Form input (coding)]

* Output
![LANGKAH 9 Form input (hasil)]

## Form Button
* Coding
![LANGKAH 10 Form Button (coding)]

* Output
![LANGKAH 10 Form Button (HASIL)]

## HTML DOM
* Coding
![LANGKAH 11 HTML DOM (coding)]

* Output
![LANGKAH 11 HTML DOM (hasil)]

# TUGAS
## 1. Buat script untuk melakukan validasi pada isian form.

* Buat form pada `lab5_javascript.html`
```
<!DOCTYPE html>
<html lang="en">
<head>
	<title>Form Validasi</title>
	<link rel="stylesheet" type="text/css" href="style.css">
    <script type="text/javascript">
        function validasiForm() {
            var nama = document.getElementById("nama").value;
            var email = document.getElementById("email").value;
            var alamat = document.getElementById("alamat").value;
            if (nama != "" && email!="" && alamat !="") {
                return true;
            }else{
                alert('Isi Alamat Anda dengan lengkap !');
                return false;
            }
        }
    </script>
</head>
<body>
	<div class="login">
		<form action="beranda.html" method="POST" onSubmit="return validasiForm()">
			<div>
				<label>Nama Lengkap:</label>
				<input type="text" name="nama" id="nama" />
			</div>
			<div>
				<label>Email:</label>
				<input type="email" name="email" id="email" />
			</div>
			<div>
				<label>Alamat:</label>
				<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
			</div>
			<div>
				<input type="submit" value="Daftar" class="tombol">
			</div>
		</form>
	</div>
</body>
</html>
```
![TUGAS (coding form validasi)]

* Buat halaman beranda `beranda.html`
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beranda</title>
    <link rel="stylesheet" href="style.css">
    <script lang="javascript">
        function pesan() {
            alert ("Selamat Datang!")
        }
    </script>
</head>
<body onload=pesan()>
    <center><h1>Terimakasih telah mendaftar!!!</h1></center>
</body>
</html>
```
![TUGAS (coding Beranda)]

* Tambahkan CSS untuk mempercantikan tampilan
```
body {
    background: darkgray;
    font-family: sans-serif;
    padding: 100px;
  }
  
  h2 {
    color: #fff;
  }
  
  .login {
    padding: 1em;
    margin: 2em auto;
    width: 17em;
    background: #fff;
    border-radius: 3px;
  }
  
  label {
    font-size: 10pt;
    color: #555;
  }
  
  input[type="text"],
  input[type="email"],
  textarea {
    padding: 8px;
    width: 95%;
    background: #efefef;
    border: 0;
    font-size: 10pt;
    margin: 6px 0px;
  }
  
  .tombol {
    background: #3498db;
    color: #fff;
    border: 0;
    padding: 5px 8px;
  }
```

