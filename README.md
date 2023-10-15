# Lab3Web
| Nama | Ahmad Hapizhudin |
-- | --
| NIM | 312210370 |

# Langkah-langkah Praktikum 
![ss6](https://github.com/hafizalkariem/Database_Penjualan_tiket_bus/assets/115614957/6bdace5f-669e-49b6-9ebb-a2495fc9f65c)

<h2 align="center" >Membuat file HTML dengan nama Lab3List.html</h2>

```html
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>HTML Lanjutan</title>
</head>
<body>
 <header>
 <h1>Membuat List</h1>
 </header>
</body>
</html>

```

## Membuat Ordered List
```html
<section id="order-list">
 <h2>Ordered List</h2>
 <ol>
 <li>Pemrograman Web</li>
 <li>Sistem Informasi</li>
 <li>Basis Data 2</li>
 </ol>
</section>

```

## Membuat Unordered List
```html
<section id="unorder-list">
 <h2>Unordered List</h2>
 <ul type="square">
 <li>Jaringan Komputer</li>
 <li>Struktur Data</li>
 <li>Algoritma &amp; Pemrograman</li>
 </ul>
</section>

```
## Membuat Description List
```html
<section id="unorder-list">
 <h2>Description List</h2>
 <dl>
 <dt>Fakultas Teknik</dt>
 <dd>Teknik Industri</dd>
 <dd>Teknik Informatika</dd>
 <dd>Teknik Lingkungan</dd>
 <dt>Fakultas Ekonomi dan Bisnis</dt>
 <dd>Akuntansi</dd>
 <dd>Manajemen</dd>
 <dd>Bisnis Digital</dd>
 </dl>
</section>
```
Setelah membuat list diatas berikut adalah hasil capturenya : 
![Screenshot 2023-10-14 224053](https://github.com/hafizalkariem/Database_Penjualan_tiket_bus/assets/115614957/203eb318-8db2-4d9e-b3f6-e00b2bf56067)

<h2 align="center" >Membuat Tabel dengan nama file lab3_tabel.html</h2> 
untuk langkah pertama sama seperti saat membuat list yaitu siapkan dulu document dengan type html. tambahkan header dibagian body

```html
<body>
 <header>
 <h1>Membuat Table</h1>
 </header>
</body>

```
## Tabel
```html
<table border="1" cellpadding="4" cellspacing="0">
 <thead>
 <tr>
 <th>No.</th>
 <th>Fakultas</th>
 <th>Program Studi</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <td>1.</td>
 <td>Teknik</td>
 <td>Teknik Informatika</td>
 </tr>
 <tr>
 <td>2.</td>
 <td>Teknik</td>
 <td>Teknik Industri</td>
 </tr>
 <tr>
 <td>3.</td>
 <td>Teknik</td>
 <td>Teknik Lingkungan</td>
 </tr>
 </tbody>
</table>
```
Berikut hasil capturenya:

![Screenshot 2023-10-15 194802](https://github.com/hafizalkariem/ProjectUAS/assets/115614957/7660d6fa-e036-46b8-b09d-cdbd943d9e71)

<h2 align="center" >Membuat Form dengan nama file lab3_form.html </h2>
Untuk membuat form pertama-tama kita tentunya membuat file dengan doctype htmlnya terlebih dahulu. setelah selesai, berikut langkah-langkah untuk membuat sebuah form :

## Form
buatlah tagar form seperti dibawah ini

```html
<form action="proses.php" method="post"></form>
```

setelah itu tambahkan beberapa tag didalamnya :

```html
<fieldset>
 <legend>Data Pelanggan</legend>
 <p>
 <label for="nama">Nama</label>
 <input type="text" id="nama" name="nama">
 </p>
 <p>
 <label for="alamat">Alamat</label>
 <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
 </p>
 <p>
 <label>Jenis Kelamin</label>
 <input id="jk_l" type="radio" name="kelamin" value="L" /><label
for="jk_l">Laki-laki</label>
 <input id="jk_p" type="radio" name="kelamin" value="P" /><label
for="jk_p">Perempuan</label>
 </p>
 <p><input type="submit" value="Login"></p>
 </fieldset>
```
Agar tampilan lebih menarik kita dapat menambahkan style css didalam tag head.

```css
<style>
 form p > label {
 display: inline-block;
 width: 100px;
 }
 form input[type="text"], form textarea {
 border: 1px solid #197a43;
 }
 form input[type="submit"] {
 border: 1px solid #197a43;
 background-color: #197a43;
 color: #ffffff;
 font-weight: bold;
 padding: 5px 15px;
 }
</style>

```

Berikut tampilan dari formnya setelah kita tambahkan style css:
![Screenshot 2023-10-15 194604](https://github.com/hafizalkariem/ProjectUAS/assets/115614957/eec6875e-c38a-49fe-aa34-f471ca6eb8b4)

# Pertanyaan dan tugas
Buatlah form yang menampilkan <b>dropdown</b> menu dan <b>listbox</b> dengan multiple selection.
## Langkah-langkah penyelesaian
Untuk membuat form dropdown menu dan listbox dengan multiple selection , caranya sama saja seperti membuat form biasa. yaitu membuat file dengan doctype html terlebih dahulu. disini kita beri nama dropdown.html .setelah itu kita buat Tagar Form terlebih dahulu:

```html
<form action="proses_form.php" method="post">
```
setelah itu kita buat fieldset yang mirip seperti saat membuat form :

```html
<fieldset class="Biodata">
        <legend>Biodata Anda</legend>
```
Buat tag label:
```html
<label for="makanan favorit" class="pilihan" >Makanan Favorit Anda</label>
<label for="minuman favorit" class="pilihan">Minuman Favorit</label>
```
Setelah itu buat tagar select untuk opsi pilihan yang akan diisi.karena perintahnya adalah membuat multiple selection  maka disini  kita juga akan membuatnya menjadi multiple selection dengan value `multiple`:

```html
<select name="makanan" id="makanan" multiple>
          <option value="1">Nasi Uduk</option>
          <option value="2">Soto Ayam</option>
          <option value="3">Sate Ayam</option>
          <option value="4">Bakso</option>
          <option value="5">Mie Ayam</option>
</select>
<select name="minuman" id="minuman" multiple>
          <option value="m1">Es Teh</option>
          <option value="m2">Es Jeruk</option>
          <option value="m3">Wedang Jahe</option>
          <option value="m4">Air Putih Biasa</option>
          <option value="m6">Lemon Tea</option>
          <option value="m7">Thai Tea</option>
          <option value="m8">Americano Coffe</option>
          <option value="m9">Starbucks</option>
          <option value="m10">Tuak</option>
</select>
```
Anda juga bisa menambahkan banyak opsi lainnya yang bisa dimasukan kedalam form dropdown tsb. setelah listnya sudah semua jangan lupa berikan tombol untuk mensubmit data yang kita isi.

```html
<input type="submit" value="submit" class="submit" />
```
