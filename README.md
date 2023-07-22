1.	Pilihan kosong/salah/tidak ditemukan
a.	Wrong Option
i.	Pemaparan: 
1.	main menu
2.	hindari
ii.	Solusi: Selalu pake if-elif-else
b.	A
c.	
2.	Case sensitive (tipe data beda)
3.	Input integer
4.	Capitalize() & title()
5.	Data Kosong
a.	Pemaparan
Pada daftar nilai siswa ini, seluruh kolom harus terisi dengan value tertentu. Tidak diperkenankan data kosong. Sama halnya pada input yang termasuk dalam fungsi CREATE & UPDATE.
b.	Permasalahan
Secara otomatis, python akan merekam value kosong apabila tidak diberi input. 
c.	Solusi
i.	Menggunakan len() == 0
Merupakan cara utama untuk mendeteksi input kosong, dimana jika terdapat data kosong, akan terus berada di dalam loop while.
CONTOH: CREATE NAMA
i.	Menggunakan isdigit
Metode isdigit() dapat dimasukkan ke dalam while loop, dimana ketika kondisi input nis berbentuk angka, langsung break dari loop.
CONTOH: REPEAT FUNCTION
ii.	While tidak langsung
Secara tidak langsung, value kosong dapat dideteksi menggunakan while loop. Contohnya adalah ketika kita ingin mengecek input jenis kelamin siswa, dimana kriteria data inputnya adalah M atau F. Data kosong, yang tidak termasuk dalam keduanya, akan termasuk dalam kategori False dan akan terus masuk ke dalam While Loop.
CONTOH: CREATE SEX
6.	Input Integer & Range - NILAI
a.	Pemaparan
Nilai suatu mata pelajaran bisa menggunakan skala huruf, seperti A, B, C, D, dan E, dan bisa juga menggunakan skala angka seperti 0-10 dan 0-100.
Nilai berskala huruf, biasanya digunakan untuk nilai sikap spiritual & social (https://www.mysch.id/blog/detail/132/contoh-deskripsi-sikap-spiritual-dan-sosial-kurikulum-2013). Sementara itu, skala angka digunakan untuk mengukur pengetahuan dari seorang siswa pada mata pelajaran eksak. Skala angka 0-100 lebih banyak digunakan karena skala nya lebih rinci dibanding 0-10.
Pada case ini, kita akan menampilkan nilai pelajaran eksak (matematika, fisika, dan kimia), sehingga digunakan skala 0-100. Sebodoh-bodoh nya seseorang, nilai minimal yang dia dapat adalah 0. Sebaliknya, sepintar-pintar nya seseorang dia mendapat nilai 100. Tidak akan ada nilai minus atau nilai lebih dari 100.
b.	Permasalahan
Dalam python ini tidak dapat secara otomatis membuat looping instruction untuk memastikan data itu berbentuk angka. 

Dimana akan menghasilkan error jika menerima input selain angka, jika dipaksakan membatasi input menjadi angka saja menggunakan int(input()) (https://www.geeksforgeeks.org/how-to-take-integer-input-in-python)

 

c.	Solusi
Perlu dipastikan yang masuk ke dalam kolom nilai mata pelajaran ini harus berbentuk angka dengan while loop isdigit() (https://www.w3schools.com/python/ref_string_isdigit.asp). Lalu selanjutnya baru dipastikan bahwa angka tersebut tidak kurang dari 0 & tidak lebih dari 100 dengan while loop test_dict[i] > 100 or test_dict[i] < 0.
7.	Nama Kepanjangan - NAMA
a.	Pemaparan
Tak seperti jaman dahulu yang hanya 1 kata saja, pada masa kini nama lengkap orang indonesia terdiri dari lebih dari 2 kata (https://jambiekspres.disway.id/read/656720/punya-momongan-tahun-2023-ini-aturan-membuat-nama-anak-sesuai-himbauan-dirjen-dukcapil-terupdate#:~:text=Minimal%20Dua%20Kata,ijazah%2C%20paspor%20dan%20lain%20sebagainya). Hal ini ditujukan agar tidak terdapat nama yang sama dalam suatu daftar nama. Nama orang juga diawali dengan huruf capital, kemudian diikuti dengan huruf kecil.
b.	Permasalahan
Meski jarang, menurut dukcapil (http://dispendukcapil.bangkalankab.go.id/baca-290-saran-dari-dukcapil-terkat-nama-anak#:~:text=Ia%20menyampaikan%20bahwa%20rata%2Drata,paling%20enak%201%2D5%20kata), terdapat nama orang Indonesia yang memiliki lebih dari 5 kata. Ketika menampilkan nya dalam daftar nama, akan sangat menyulitkan karena akan sangat memakan banyak space.
c.	Solusi
Jika total karakter dalam nama lengkap lebih dari 30 char, kita akan menyingkat nama orang tersebut dengan hanya memasukkan 3 kata awal saja. Kemudian kata ke-4 dan seterusnya akan disingkat dengan hanya memasukkan inisialnya (huruf terdepan) saja.

CONTOH: 
Boyke Adhitya Yudhya Leon Augusta -> Boyke Adhitya Yudhya L A
Muhammad Fadhil Abdul Baasith -> Muhammad Fadhil Abdul B

Untuk membuat huruf pertama di setiap kata menjadi huruf kapital, kita gunakan fungsi title() & capitalize().

8.	Variabel global
a.	Pemaparan
Ada berbagai fungsi pada program CRUD yang dipanggil berulang kali. Dalam daftar nilai siswa ini, NIS yang merupakan primary-key dipanggil berulang kali dalam fungsi Create, Read, Update, dan Delete.
b.	Permasalahan
Pastinya akan sangat membuang space jika menulis fungsi tersebut berulang kali.
c.	Solusi
Membuat fungsi tersendiri dengan memanggil nis sebagai variable global (https://www.w3schools.com/python/python_variables_global.asp)

 

