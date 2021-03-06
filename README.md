# Praktikum 2 - Prmorgaman Web ( CSS Dasar )
```
Mochamad Amri Adrian Wiratama
311910226
TI. 19. A2
Universitas Pelita Bangsa
```
## Langkah 1
Membuat dokumen HTML sebagai berikut :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
</head>
<body>
    <header>
        <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a href="lab1_tag-dasar.html">Dasar HTML</a>
    </nav>
    <!-- CSS ID Selector-->
    <div id="intro">
        <h1>Hello World</h1>
        <p>>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b>di<i>Universitas Pelita Bangsa</i>. Pelajaraan pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag - tag dasar HTML dan CSS</p>
        <!-- CSS IS Selector -->
    <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
    </div>
</body>
</html>
```
![Langkah 1](https://user-images.githubusercontent.com/56380838/113967503-4e6acc80-985b-11eb-8ae3-3d149cd59efd.png)
## Langkah 2
Setelah itu tanbahkan deklarasi CSS internal dalam bagian `<head>` dokumen.
```
<head>
<style>
        body {
            font-family: 'Open Sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom: 1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color:#6d6a6b;
        }
 </style>
 </head>
 ```
![Langkah 2](https://user-images.githubusercontent.com/56380838/113967517-56c30780-985b-11eb-94ca-7e91845f2276.png)
## Langkah 3
Mendeklarasikan inline CSS pada paragraf atau tag `<p>`.
```
<p style="text-align: center; color: #ccd8e4;">
```
![Langkah 3](https://user-images.githubusercontent.com/56380838/113967535-5e82ac00-985b-11eb-9745-3d6d53ee2125.png)
## Langkah 4
Membuat CSS eksternal dan Kemudian tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagian `<head>`.
```
nav {
    background: #20A759;
    color: #fff;
    padding: 10px;
}
nav a {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
}
nav .active,
nav a:hover{
    background: #0B6B3A;
}
```
```
<!--Menyisipkan css eksternal-->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
```
![Langkah 4,](https://user-images.githubusercontent.com/56380838/113969664-95f35780-985f-11eb-855c-eb23c2e67db5.png)
Setelah browser di refresh
![Langkah 4 2](https://user-images.githubusercontent.com/56380838/113967589-73f7d600-985b-11eb-86f5-5df3286c519e.png)
## Langkah 5
Menambah CSS Selector dengan menggunakan ID dan Class Selector pada dokumen css eksternal.
```
/* ID Selector */
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
}
#intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
}
/* Class Selector */
.botton {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
}
.btn-primary {
    background: #e42a42;
}
```
![Langkah 5](https://user-images.githubusercontent.com/56380838/113970737-955bc080-9861-11eb-9f0f-3c7b39f3f0b5.png)
# Pertanyaan :
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
```
Saya melakukan beberapa eksperimen seperti mengubah nilai yang hasilnya mengubah ukuran ataupun warna dan mengganti background.

```
![Eksperimen 2](https://user-images.githubusercontent.com/56380838/114653281-e4966b00-9d11-11eb-8e6c-be77b3bef887.png)
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
```
Pendeklarasian CSS elemen h1 mengubah tampilan seluruh elemen yang memiliki tag h1, sedangkan #intro h1 hanya mengubah tampilan elemen h1 yang memiliki id #intro.
```
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser?Berikan penjelasan dan contohnya!
```
Setelah saya mencoba, jika mendeklarasikan CSS pada elemen yang sama namun dengan isi deklarasi yang berbeda, maka semua deklarasi CSS tersebut akan ditampilkan. Contohnya:
```
![Pertanyaan 3](https://user-images.githubusercontent.com/56380838/114668338-d1dc6000-9d2a-11eb-8fd8-f765b3ac444b.png)
![Pertanyaan 3,2](https://user-images.githubusercontent.com/56380838/114668399-e4569980-9d2a-11eb-805b-d8df3b174e6b.png)
```
Namun jika isi dari ketiga deklarasi CSSnya sama semua, maka browser hanya akan menampilkan salah satunya, dengan urutan Inline CSS, Eksternal CSS, dan yang terakhir Internal CSS
```
![Pertanyaan 3,3](https://user-images.githubusercontent.com/56380838/114668443-f20c1f00-9d2a-11eb-92e2-c277cddf9b92.png)
![Pertanyaan 3,4](https://user-images.githubusercontent.com/56380838/114668456-f6383c80-9d2a-11eb-8057-da304dbe4a2e.png)


5. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
```
Kedua deklarasi tersebut akan tampil, namun selector ID yang akan tampil jika deklarasinya ada yang sama antara ID dan Class.
```
![Pertanyaan 5](https://user-images.githubusercontent.com/56380838/114673125-11597b00-9d30-11eb-83b8-4d87b6913ebb.png)

