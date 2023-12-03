# Lab9Web

---

# Langkah Langkah Pratikum

Buatlah file baru dengan nama `Header.php`

`Untuk codenya bisa menggunakan dibawah ini:`

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Contoh Modularisasi</title>
    <link href="style.css" rel="stylesheet" type="text/stylesheet" media="screen" />
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
        </nav>
```

# Selanjutnya buatlah file baru dengan nama `footer.php`

`Untuk codenya bisa menggunakan dibawah ini:`

```html
<footer>
    <p>&copy; 2021, Informatika, Universitas Pelita Bangsa</p>
</footer>
</div>
</body>

</html>
```
# Selanjutnya buatlah file baru dengan nama `home.php`

`Untuk codenya bisa menggunakan dibawah ini:`

```html
<?php require('header.php') ?>
<div class="content">
    <h2>Ini Halaman home</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>
<?php require('footer.php'); ?>
```
# Selanjutnya buatlah file baru dengan nama `about.php`

`Untuk codenya bisa menggunakan dibawah ini:`

```html
<?php require('header.php'); ?>
<div class="content">
    <h2>Ini Halaman About</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>
<?php require('footer.php'); ?>
```

