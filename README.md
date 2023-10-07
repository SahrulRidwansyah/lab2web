# lab2web

```
Sahrul Ridawansyah
312210063
```

# 1. Membuat dokumen HTML

![image](https://github.com/sahrul180304/lab2web/assets/115526901/34404755-9714-4674-9a4e-4c96c5616e9d)


# 2. Mendeklarasikan CSS Internal

![image](https://github.com/sahrul180304/lab2web/assets/115526901/2be312ca-04aa-4887-a25a-54c686bcef2d)


# 3. Menambahkan Inline CSS

![image](https://github.com/sahrul180304/lab2web/assets/115526901/b173b910-813c-4094-8e80-3534a0e36c69)


# 4. Membuat CSS Eksternal

![image](https://github.com/sahrul180304/lab2web/assets/115526901/6bdad523-e774-400a-be98-7ebd1373b6d0)


# 5. Menambahkan CSS Selector

![image](https://github.com/sahrul180304/lab2web/assets/115526901/48103d9e-8dd9-40f8-8ff0-b1f8b888ac17)


# 6. validasi dokumen css

![image](https://github.com/sahrul180304/lab2web/assets/115526901/40b4fe14-fdfd-4340-8852-58e66ab483da)



# Pertanyaan dan Tugas

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

jawaban: 

![image](https://github.com/sahrul180304/lab2web/assets/115526901/00d4cf3f-dab1-465b-93f9-01ef935ef59f)


2. Apa perbedaan pendeklarasian CSS elemen `h1` `{...}` dengan #intro `h1` `{...}`? berikan
penjelasannya!

jawaban:

Berikut adalah penjelasan perbedaannya:

`h1` `{...}`:

- Pendeklarasian ini akan mempengaruhi semua elemen `<h1>` di seluruh halaman web.
  
- Ini adalah contoh dari pemilihan elemen berdasarkan jenisnya `(tag selector)`. 

- Ini akan mengubah semua elemen `<h1>` di halaman tanpa memandang di mana elemen-elemen tersebut berada dalam struktur dokumen HTML.

Contoh penggunaannya adalah jika Anda ingin mengubah gaya teks semua elemen `<h1>` di seluruh situs web, seperti mengubah warna teks, ukuran font, atau gaya lainnya secara konsisten.

#intro `h1` `{...}`:

- Pendeklarasian ini akan mempengaruhi elemen `<h1>` yang berada dalam elemen dengan id "intro".
  
- Ini adalah contoh dari pemilihan elemen berdasarkan hierarki atau "nested selector".
  
- Ini akan mengubah gaya elemen `<h1>` yang berada dalam elemen dengan id "intro" saja.
  
Contoh penggunaannya adalah jika Anda memiliki elemen `<h1>` yang hanya ingin Anda ubah gayanya ketika elemen tersebut berada dalam konteks elemen dengan id "intro". Ini memungkinkan Anda untuk memberikan gaya khusus pada elemen tersebut dalam konteks tertentu.


3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!

jawaban:

etika Anda memiliki deklarasi CSS yang dideklarasikan secara internal `(di dalam tag `<style>` dalam elemen `<head>`)`, CSS eksternal `(di dalam file eksternal dengan ekstensi .css)`, dan CSS inline `(langsung dalam atribut style elemen HTML yang bersangkutan)` yang mempengaruhi elemen yang sama, prinsip "specificity" dan urutan pengaturan akan mempengaruhi deklarasi mana yang akan ditampilkan oleh browser.

Contoh:

`<p id="paragraf" class="teks-merah" style="color: blue;">`Ini adalah teks paragraf.`</p>`

Dan ada CSS yang terkait:

CSS Internal:

`<style>`
  p `{
    color: green;
  }`
`</style>`

CSS Eksternal `(styles.css)`:

.teks-merah `{
  color: red;
}`


4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! `( `<p id="paragraf-1" class="text-paragraf">` )`

jawaban:

Ketika sebuah elemen HTML memiliki baik ID maupun Class, deklarasi CSS yang akan ditampilkan oleh browser akan dipengaruhi oleh kombinasi dari keduanya. Namun, perlu diingat bahwa ID 

memiliki prioritas yang lebih tinggi daripada Class. Berikut adalah penjelasan lebih lanjut dan contohnya:

`<p id="paragraf-1" class="text-paragraf">`Ini adalah teks paragraf.`</p>`

Jika ada deklarasi CSS sebagai berikut:

#paragraf-1 `{
  color: red;
}`

.text-paragraf `{
  color: blue;
}`

alam kasus ini, deklarasi CSS dengan ID selector `(#paragraf-1)` akan memiliki prioritas tertinggi. Oleh karena itu, warna teks paragraf ini akan menjadi merah, sesuai dengan deklarasi color: red;. Deklarasi CSS dengan class selector `(text-paragraf)` akan diabaikan dalam hal ini karena ID selector memiliki prioritas yang lebih tinggi.

Jadi, pada elemen HTML `<p id="paragraf-1" class="text-paragraf">`, deklarasi CSS yang akan ditampilkan adalah color: red; karena ID selector `(#paragraf-1)` memiliki prioritas yang lebih tinggi daripada class selector `(text-paragraf)`.


