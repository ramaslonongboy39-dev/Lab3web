## Langkah-Langkah Praktikum

### 1. Membuat Dokumen HTML

Pada langkah pertama dibuat struktur dasar HTML yang terdiri dari header, navigation, dan bagian intro.

### Screenshot

![Langkah 1 - Membuat Dokumen HTML]!(<Screenshot 2026-10-05 110731.png>)

---

### 2. Menambahkan CSS Internal 

Selanjutnya ditambahkan CSS Internal menggunakan tag `<style>` pada bagian `<head>`. CSS digunakan untuk mengatur font, header, heading, warna, dan posisi teks.

### Screenshot

![Langkah 2 - CSS Internal]!(<Screenshot 2026-10-05 111029.png>)
---

### 3. Menambahkan Inline CSS

Pada langkah ini ditambahkan Inline CSS secara langsung pada elemen `<p>` menggunakan atribut `style`.

### Screenshot

![Langkah 3 - Inline CSS]!(<Screenshot 2026-10-05 111620.png>)

---

### 4. Membuat CSS Eksternal

Selanjutnya dibuat file `style_eksternal.css` dan dihubungkan dengan file HTML menggunakan tag `<link>`.

### Screenshot

![Langkah 4 - CSS Eksternal]!(<Screenshot 2026-10-05 112427.png>)

---

### 5. Menambahkan CSS Selector

Pada langkah terakhir digunakan beberapa selector CSS, yaitu Element Selector, ID Selector, dan Class Selector.

### Screenshot

![Langkah 5 - CSS Selector]!(<Screenshot 2026-10-05 113211.png>)

---

## Hasil Akhir

Berikut adalah hasil akhir dari praktikum CSS Dasar.

![Hasil Akhir]!(<Screenshot 2026-10-05 113918.png>)

## Kesimpulan

Dari praktikum ini dapat dipahami penggunaan CSS untuk mengatur tampilan halaman HTML. CSS dapat diterapkan menggunakan Internal CSS, Inline CSS, dan External CSS.

Selain itu, dipelajari juga penggunaan Element Selector, ID Selector, dan Class Selector untuk mengatur elemen-elemen pada halaman web.

## Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline
CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector
tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada
browser? Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-
paragraf"> )



## JAWABAN SOAL

## Jawaban Soal 1
Saya melakukan eksperimen dengan mengubah beberapa properti CSS seperti font-family, background-color, color, font-size, text-align, dan line-height.
Contoh:
body {
font-family: Arial, sans-serif;
background-color: #f4f4f4;
}

h1 {
color: blue;
text-align: center;
font-size: 28px;
}

p {
color: black;
font-size: 18px;
line-height: 1.6;
}

Perubahan tersebut digunakan untuk melihat pengaruh property dan value CSS terhadap tampilan halaman web.

## Jawaban Soal 2

Perbedaan h1 { ... } dengan #intro h1 { ... } terletak pada cakupan elemen yang diberikan CSS.

h1 { ... } akan memberikan style kepada semua elemen <h1> yang terdapat pada halaman.

Contoh:

h1 {
color: red;
}

Sedangkan:

#intro h1 {
color: blue;
}

hanya memberikan style kepada elemen <h1> yang berada di dalam elemen yang memiliki ID intro.

Contoh HTML:

<div id="intro">
    <h1>Hello World</h1>
</div>

Jadi, h1 memiliki cakupan yang lebih umum, sedangkan #intro h1 lebih spesifik karena hanya berlaku pada <h1> yang berada di dalam #intro.

## Jawaban Soal 3

Jika sebuah elemen memiliki CSS Internal, CSS Eksternal, dan Inline sekaligus, maka Inline CSS memiliki prioritas lebih tinggi dibandingkan CSS Internal dan CSS Eksternal pada kondisi aturan yang sama.

Contoh CSS Eksternal:

p {
color: blue;
}

CSS Internal:

<style>
    p {
        color: green;
    }
</style>

Inline CSS:

<p style="color: red;">
    Belajar CSS
</p>

Hasil yang ditampilkan pada browser adalah teks berwarna merah, karena color: red ditulis secara langsung pada atribut style elemen tersebut.

## Jawaban Soal 4

Jika sebuah elemen HTML memiliki ID dan Class, kemudian keduanya memiliki aturan CSS yang berbeda, maka ID Selector memiliki prioritas lebih tinggi daripada Class Selector.

Contoh:

.text-paragraf {
color: blue;
}

#paragraf-1 {
color: red;
}

HTML:

<p id="paragraf-1" class="text-paragraf">
    Ini adalah paragraf.
</p>

Hasilnya adalah teks akan berwarna merah, karena selector ID #paragraf-1 memiliki spesifisitas lebih tinggi daripada selector class .text-paragraf.