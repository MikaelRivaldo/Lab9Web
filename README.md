# Lab9Web

---

# Langkah Langkah Pratikum


# Tugas

Implementasikan konsep modularisasi pada kode program praktikum 8

Buat file baru dengan nama header.php

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Contoh Modularisasi</title>
    <style>
        * {
            padding: 0;
            margin: 0;
            font-family: "Roboto", sans-serif;
        }

        body {
            margin: 0;
            padding: 0;
            height: 611px;
            position: relative;
        }

        nav {
            width: 100%;
            background-color: #8A2BE2;
            padding: 0px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        nav>a {
            text-decoration: none;
            color: white;
            padding: 10px;
            margin: 10px 5px;
            border-radius: 5px;
        }

        nav>a:hover,
        nav>a.active {
            background-color: rgb(4, 149, 237);
        }

        header {
            text-align: center;
            padding: 30px;
        }

        header code {
            color: crimson;
        }

        .content {
            background-color: rgb(165, 165, 165);
            color: white;
            width: 90%;
            margin: auto;
            margin-bottom: 50px;
            padding: 20px;
            border-radius: 5px;
        }

        .content h2 {
            margin-bottom: 20px;

        }

        .content span {
            color: rgb(52, 55, 57);
        }

        footer {
            position: absolute;
            bottom: 0;
            width: 100%;
            background-color: #8A2BE2;
            text-align: center;
            padding: 20px 0;
            color: white;
        }
    </style>
</head>

<body>
    <div class="container">
        <header>
            <h1>Modularisasi Menggunakan Require</h1>
        </header>
        <nav>
            <a href="home.php">Home</a>
            <a href="about.php">Tentang</a>
            <a href="kontak.php">Kontak</a>
            <a href="data_barang.php">Data barang</a>
        </nav>
        <?php require('footer.php'); ?>
```

Untuk hasilnya akan seperti ini:

![image](https://github.com/MikaelRivaldo/Lab9Web/assets/115770247/5958890a-48ba-4560-b7c1-70e70f966c75)

`NOTE` tampilan diatas adalah header dan footer

# Selanjutnya buatlah file baru dengan nama `footer.php`

`Untuk codenya bisa menggunakan dibawah ini:`

```html
<footer>
    <p>&copy; 2021, Informatika, Mikael Rivaldo Universitas Pelita Bangsa</p>
</footer>
</div>
</body>

</html>
```
# Selanjutnya buatlah file baru dengan nama `about.php`

<?php require('header.php'); ?>
<div class="content">
    <h2>Ini Halaman About</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>
<?php require('footer.php'); ?>

Untuk hasilnya akan seperti ini:

![image](https://github.com/MikaelRivaldo/Lab9Web/assets/115770247/40185a46-0ff0-47b4-b660-5a567d86baa6)


# Selanjutnya buatlah file baru dengan nama `kontak.php`

```html
<?php require('header.php'); ?>
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        /* Kontak */
        .contact-form {
            width: 300px;
            margin: auto;
            margin-top: -40px;
        }

        .form-group label {
            display: block;
            margin-bottom: 1px;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
        }

        .form-group textarea {
            height: 100px;
        }

        .submit-btn {
            width: 100%;
            padding: 10px;
            background-color: rgb(44, 174, 253);
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 20px;
        }

        .submit-btn:hover {
            background-color: rgb(138, 142, 146);
        }
    </style>
</head>

<body>
    <div class="content">
        <h2>Ini Halaman <span>Kontak</span></h2>
        <p>Ini adalah bagian content dari halaman.</p>
    </div>
    <div class="contact-form" id="kontak"> <!--Kontak-->
        <h2>Contact Us</h2>
        <form action="#" method="post">
            <div class="form-group">
                <label for="name">Nama:</label>
                <input type="text" id="name" name="name" required>
            </div>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
            </div>
            <div class="form-group">
                <label for="message">Pesan:</label>
                <textarea id="message" name="message" required></textarea>
            </div>
            <button type="submit" class="submit-btn">Kirim Pesan</button>
        </form>
    </div>
</body>

</html>
<?php require('footer.php'); ?>
```
Untuk hasilnya akan seperti ini:

![image](https://github.com/MikaelRivaldo/Lab9Web/assets/115770247/c8d1df5f-62f1-49d6-9e03-6ea3e1ac98a9)
