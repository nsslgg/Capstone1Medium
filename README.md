1.	Pilihan kosong/salah/tidak ditemukan
a.	Wrong Option
i.	Pemaparan: 
1.	main menu
2.	hindari
ii.	Solusi: Selalu pake if-elif-else
b.	A
c.	
2.	Case sensitive (tipe data beda)
3.	Range
a.	Pemaparan
Nilai suatu mata pelajaran bisa menggunakan skala huruf, seperti A, B, C, D, dan E, dan bisa juga menggunakan skala angka seperti 0-10 dan 0-100.
Nilai berskala huruf, biasanya digunakan untuk nilai sikap spiritual & social (https://www.mysch.id/blog/detail/132/contoh-deskripsi-sikap-spiritual-dan-sosial-kurikulum-2013). Sementara itu, skala angka digunakan untuk mengukur pengetahuan dari seorang siswa melalui ujian tulis. Skala angka 0-100 lebih banyak digunakan karena skala nya lebih rinci dibanding 0-10.
Pada case ini, kita akan menampilkan nilai pelajaran eksak (matematika, fisika, dan kimia, sehingga digunakan skala 0-100. Sebodoh-bodoh nya seseorang, nilai minimal yang dia dapat adalah 0. Sebaliknya, sepintar-pintar nya seseorang dia mendapat nilai 100. Tidak akan ada nilai minus atau nilai lebih dari 100.
b.	Permasalahan
Dalam python ini tidak dapat secara otomatis membuat looping untuk memastikan data itu berbentuk angka. Dimana akan menghasilkan error.
 ![image](https://github.com/nsslgg/Capstone1Medium/assets/121706256/ee025b05-f145-4a90-bc84-75a7818bbe3b)

c.	Solusi
Perlu dipastikan yang masuk ke dalam kolom nilai mata pelajaran ini harus berbentuk angka dengan isdigit() (https://www.w3schools.com/python/ref_string_isdigit.asp). Kemudian harus dipastikan bahwa angka tersebut tidak kurang dari 0 & tidak lebih dari 100.
4.	Nama Kepanjangan
a.	Pemaparan
Tak seperti jaman dahulu yang hanya 1 kata saja, pada masa kini nama lengkap orang indonesia terdiri dari lebih dari 2 kata (https://jambiekspres.disway.id/read/656720/punya-momongan-tahun-2023-ini-aturan-membuat-nama-anak-sesuai-himbauan-dirjen-dukcapil-terupdate#:~:text=Minimal%20Dua%20Kata,ijazah%2C%20paspor%20dan%20lain%20sebagainya). Hal ini ditujukan agar tidak terdapat nama yang sama dalam suatu daftar nama.
b.	Permasalahan
Meski jarang, menurut dukcapil (http://dispendukcapil.bangkalankab.go.id/baca-290-saran-dari-dukcapil-terkat-nama-anak#:~:text=Ia%20menyampaikan%20bahwa%20rata%2Drata,paling%20enak%201%2D5%20kata), terdapat nama orang Indonesia yang memiliki lebih dari 5 kata. Ketika menampilkan nya dalam daftar nama, akan sangat menyulitkan karena akan sangat memakan banyak space.
c.	Solusi
Jika total karakter dalam nama lengkap lebih dari 30, kita akan menyingkat nama orang tersebut dengan hanya memasukkan 3 kata awal saja. Kemudian kata ke-4 dan seterusnya akan disingkat dengan hanya memasukkan inisialnya (huruf terdepan) saja.
Contoh: 
Boyke Adhitya Yudhya Leon Augusta -> Boyke Adhitya Yudhya L A
Muhammad Fadhil Abdul Baasith -> Muhammad Fadhil Abdul B

5.	Variabel global
Ada berbagai fungsi pada program CRUD yang dipanggil berulang kali.
a.	
