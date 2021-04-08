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

![Langkah 4 2](https://user-images.githubusercontent.com/56380838/113967589-73f7d600-985b-11eb-86f5-5df3286c519e.png)
![Langkah 5](https://user-images.githubusercontent.com/56380838/113967594-78bc8a00-985b-11eb-8a20-7cd33c9efea9.png)
