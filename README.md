# Jobhseet 2 - Routing, Controller, dan View

Nama : Shasia Sasa Salsabyla \
Kelas : TI - 2F \
No.Absen/NIM : 25/2241720029

## Basic Routing

1.  Route Hello \
    ![alt text](gambar/1.png) \
     Halaman muncul tulisan Hello Word, sesuai dengan apa yang diketikkan di file web.php

          Route::get('/hello', function () { return 'Hello World'; });

2.  Route World \
    ![alt text](gambar/2.png) \
    Halaman menampilkan tulisan World sesuai dengan

          Route::get('/world', function () { return 'World'; });

3.  Route Index\
    ![alt text](gambar/3.png)

4.  Route About \
    ![alt text](gambar/4.png)

## Route Parameters

1. Route User \
   ![alt text](gambar/5.png) \
   Halaman menampilkan "Nama saya Shasia" dengan mengetikkan URL localhost/PWL_2024/public/user/Shasia. "Shasia" ditampilkan dari apa yang diketikkan di URL.

2. Route User (Not Found) \
   ![alt text](gambar/6.png) \
   Sama seperti sebelumnya, tapi karena URL tidak dilengkapi nama sehingga tidak menemukan halaman yang dicari dan menampilkan halaman 404 Not Found.

3. Route Comments \
   ![alt text](gambar/7.png) \
   Sama seperti sebelumnya. Namun disini route bisa menerima lebih dari 1 parameter. Route menerima parameter $postId dan juga $comment.

4. Route Articles \
   ![alt text](gambar/8.png)

## Optional Parameters

1. User (Null) \
   ![alt text](gambar/9.png) \
   Karena disini diberi keterangan nama = null, sehingga jika pada URL tidak diberi "nama" maka hanya menampilkan "Nama saya" tanpa ada yang dipanggil.

2. User/Shasia \
   ![alt text](gambar/10.png) \
   Sama seperti sebelumnya, namun disini diketikkan "nama" pada URL

3. User \
   ![alt text](gambar/11.png) \
   Menampilkan "Nama saya John" karena sudah ditentukan pada kode programnya.

## Controller

1. Membuat Controller \
   ![alt text](gambar/12.png)

2. Controller Hello \
   ![alt text](gambar/13.png) \
   Menampilkan halaman web dengan tulisan "Hello World". Disini menggunakan controller agar lebih terstruktur.

3. Modifikasi \
   ![alt text](gambar/28.png) \
   ![alt text](gambar/29.png) \
   ![alt text](gambar/14.png) \
   ![alt text](gambar/15.png) \
   ![alt text](gambar/16.png)

4. Modifikasi Single Action Controller

    ![alt text](gambar/17.png) \
    ![alt text](gambar/18.png) \
    ![alt text](gambar/19.png) \
    ![alt text](gambar/30.png) \
    ![alt text](gambar/20.png) \
    ![alt text](gambar/31.png) \
    ![alt text](gambar/21.png) \
    ![alt text](gambar/32.png)

## Resource Controller

1. Membuat Controller \
   ![alt text](gambar/22.png)

2. List Route \
   ![alt text](gambar/23.png)

## View

1. View \
   ![alt text](gambar/24.png) \
   Menampilkan "Hello, Shasia" dengan menggunakan view, dengan route memanggil view sesuai dengan nama file.

2. View dalam Direktori \
   ![alt text](gambar/25.png) \
   Disini menyimpan file view dalam direktori blog. Menampilkan halaman yang sama seperti sebelumnya.

3. View dari Controller \
   ![alt text](gambar/26.png) \
   Menggunakan controller untuk memanggil view. Routing akan memanggil controller terlebih dahulu, kemudian akan me-return view yang dituju.

4. Meneruskan Data ke View \
   ![alt text](gambar/27.png) \
   Meneruskan data array ke view agar data tersebut tersedia untuk view. Tampilan sama seperti sebelumnya dengan tambahan array.
