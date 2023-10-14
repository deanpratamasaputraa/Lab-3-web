# Lab3Web

Nama : Dean Pratama Saputra

NIM  : 312210114

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksi-praktikum)|
|2|Praktikum|[Click Here](#praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Instruksi Praktikum
> 1. Persiapkan text editor misalnya VSCode.
> 2. Buat folder baru dengan nama Lab3Web
> 3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
> 4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## Praktikum
**1. Membuat Ordered List & Undordered List**

```
<section id="order-list">
  <h2>Ordered List</h2>
  <ol>
    <li>Pemrograman Web</li>
    <li>Sistem Informasi</li>
    <li>Basis Data 2</li>
  </ol>
</section>
```

<img width="960" alt="membuat list" src="https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/a8274ecc-d6be-4667-8d92-9204a17b346a">



```
<section id="unorder-list">
  <h2>Unordered List</h2>
  <ul type="square">
    <li>Jaringan Komputer</li>
    <li>Struktur Data</li>
    <li>Algoritma &amp; Pemrograman</li>
  </ul>
</section>
```

<img width="960" alt="membuat list" src="https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/5426fa44-0983-40f6-91b0-76d503953dec">



**2. Membuat Description List**

```
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

<img width="960" alt="membuat list" src="https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/b148dc5a-9af8-4fe5-83c5-305b746a2cad">



**3. Membuat Table**

```
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

![Screenshot (20)](https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/8ebb8ec9-4480-4bdf-a1c8-45c40221bc82)



**4. Membuat Margin dan Padding**

```
<table border="1" cellpadding="4" cellspacing="0"></table>
```

![Screenshot (20)](https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/fcace294-e625-4b0c-9986-c18b3fb49899)



**5. Menggabungkan Sel Data**

```
<tr>
  <td>1.</td>
  <td rowspan="3">Teknik</td>
  <td>Teknik Informatika</td>
</tr>
```

![Screenshot (20)](https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/34327e41-282e-46cf-abd7-105ea416f910)



**6. Membuat Form**

```
<form action="proses.php" method="post">
  <fieldset>
    <legend>Data Pelanggan</legend>
    <p>
      <label for="nama">Nama</label>
      <input type="text" id="nama" name="nama" />
    </p>
    <p>
      <label for="alamat">Alamat</label>
      <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
      <label>Jenis Kelamin</label>
      <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l"
        >Laki-laki</label
      >
      <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        qafor="jk_p"
        >Perempuan</label
      >
    </p>
    <p><input type="submit" value="Login" /></p>
  </fieldset>
</form>
```

<img width="960" alt="membuat form" src="https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/24efeae6-8901-4bfd-9902-eff4a327cf6e">



**7. Menambahkan Style**

```
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

<img width="960" alt="membuat form" src="https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/d2bb1e55-9d55-4cb9-b725-6ace50be85d6">



## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan **dropdown** menu dan **listbox** dengan *multiple selection.*

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tugas Form Dropdown and Listbox</title>
    <link rel="style" href="style.css">
</head>

<body>
    <nav>
        <a href="lab3_list.html">List HTML</a>
        <a href="lab3_tabel.html">Tabel HTML</a>
        <a href="lab3_form.html">Form HTML</a>
        <a href="lab3_tugas.html">Form Dropdown & Listbox</a>
    </nav>
    <header>
        <h1>Form Dropdown & Listbox</h1>
    </header>

    <form class="form_tugas">
        <label for="dropdown">Pilih salah satu buah:</label>
        <select name="dropdown" id="dropdown">
            <option value="apel">Apel</option>
            <option value="jeruk">Jeruk</option>
            <option value="durian">Durian</option>
            <option value="mangga">Mangga</option>
            <option value="semangak">Semangka</option>
        </select>

        <br><br>

        <label for="listbox">Pilih beberapa buah:</label>
        <select name="buah[]" multiple id="listbox">
            <option value="apel">Apel</option>
            <option value="jeruk">Jeruk</option>
            <option value="durian">Durian</option>
            <option value="mangga">Mangga</option>
            <option value="semangka">Semangka</option>
            <option value="kelapa">Kelapa</option>
            <option value="anggur">Anggur</option>
            <option value="melon">Melon</option>
            <option value="pepaya">Pepaya</option>
            <option value="nanas">Nanas</option>
        </select>

        <br>

        <input type="submit" value="Submit" id="input_tugas">
    </form>
</body>

</html>
```

```
body {
    font-family: Tahoma;
  }
  
  h1 {
    margin-top: 50px;
    text-align: center;
    color: #3d9a38;
  }
  
  .tabel {
    margin: 20px auto;
  }
  
  form p > label {
    display: inline-block;
    width: 100px;
  }
  
  form input[type="text"],
  form textarea {
    border: 1px solid #4dacd1;
  }
  
  form input[type="submit"] {
    border: 1px solid #84a9d4;
    background-color: #5375b9;
    color: #da8383;
    font-weight: bold;
    padding: 5px 15px;
    border-radius: 10px;
  }
  
  form input[type="submit"]:hover {
    background-color: #2098cb;
    cursor: pointer;
  }
  
  nav {
    background-color: #3fb8e0c5;
    padding: 10px;
    position: fixed;
    top: 0px;
    right: 0px;
    left: 0px;
    text-align: center;
  }
  
  nav a {
    color: #fff;
    text-decoration: none;
    padding: 2px 4px;
    font-size: 13px;
  }
  
  nav a:hover {
    color: #487689;
  }
  
  nav a:active {
    color: #3dd274;
  }
  
  /* Style untuk form dropdown & listbox */
  .form_tugas {
    max-width: 400px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #a9e664;
    background-color: #eb9ee1;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  
  /* Style untuk label */
  .form_tugas label {
    display: block;
    font-weight: bold;
    margin-bottom: 5px;
  }
  
  /* Style untuk select dropdown dan listbox */
  .form_tugas select {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #be77a7;
    border-radius: 3px;
  }
  
  /* Style untuk tombol Submit */
  .form_tugas #input_tugas {
    background-color: #6caaed;
    color: #984f4f;
    padding: 5px 15px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
  }
  
  .form_tugas #input_tugas:hover {
    background-color: #d469ca;
  }
```

<img width="960" alt="memilih buah" src="https://github.com/deanpratamasaputraa/Lab-3-web/assets/120002341/d1ba2503-2ff3-4b0f-b2eb-127174388d0e">



## Finish, Terima Kasih
