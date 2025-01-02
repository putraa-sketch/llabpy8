# LAPORAN LATIHAN STRING


## CODE PROGRAM STRING

### Step 1 : 
Kode ini mengimpor library re (regular expression) yang digunakan untuk pencocokan pola pada string. Dalam program ini, library ini digunakan untuk memvalidasi nama.

Selain itu, Method _init_ adalah konstruktor yang dijalankan saat objek kelas dibuat. Di sini, atribut data_mahasiswa diinisialisasi sebagai list kosong untuk menyimpan data mahasiswa.

![Screenshot 2025-01-02 111605](https://github.com/user-attachments/assets/71cf4a6d-4369-4fc8-ae8a-797192aaff0d)


### Step 2 : 
Fungsi ini digunakan untuk memvalidasi data pendaftaran. Parameter name, phone, dan email adalah input pengguna. Sebuah list kosong bernama errors disiapkan untuk menyimpan pesan kesalahan jika ada.

![Screenshot 2025-01-02 111926](https://github.com/user-attachments/assets/960217e0-bcb3-4b14-98ae-d80ef93de266)


- Validasi Nama : re.match(r'^[A-Za-z\s]+$', name) memeriksa apakah nama hanya berisi huruf (A-Z atau a-z) dan spasi (\s), Jika nama tidak sesuai dengan pola tersebut, pesan kesalahan ditambahkan ke list errors.

![Screenshot 2025-01-02 111943](https://github.com/user-attachments/assets/e5288135-3766-403b-bff5-6f8fd12407d6)


- Validasi Nomor Telepon : phone.isdigit() memeriksa apakah input nomor telepon hanya terdiri dari angka, Jika ada karakter lain (seperti huruf atau simbol), pesan kesalahan ditambahkan.

![Screenshot 2025-01-02 112002](https://github.com/user-attachments/assets/2d0bb038-3f40-416f-b72c-19e8da625bdb)


- Validasi Email : Memeriksa apakah email mengandung simbol (@) dan (.) Jika tidak, pesan kesalahan ditambahkan.

![Screenshot 2025-01-02 112035](https://github.com/user-attachments/assets/ab8392ac-f15d-4fd9-b074-5379ea5dec29)


### Step 3 :
Jika terdapat kesalahan (list errors tidak kosong), setiap pesan kesalahan ditampilkan satu per satu, Jika tidak ada kesalahan, program menampilkan pesan bahwa data pendaftaran valid.

![Screenshot 2025-01-02 112346](https://github.com/user-attachments/assets/74f9bd4c-81fc-424d-b22e-ac01f152259b)


### Step 4 :
Program meminta pengguna untuk memasukkan:
- Nama lengkap (name)
- Nomor telepon (phone)
- Email (email)

![Screenshot 2025-01-02 112507](https://github.com/user-attachments/assets/cb56b9c4-2f5c-4c0b-bb33-17f69b241ee7)


### Step 5 :
Input dari pengguna dikirim ke fungsi validate_registration untuk diperiksa validitasnya.
 
<img width="418" alt="image" src="https://github.com/user-attachments/assets/17f90766-ac6b-4a56-a1ef-faf96cd456a0" />



### Step 6 : 
Tahap akhir adalah uji coba code program yang sudah dibuat dengan mencoba berbagai kemungkinan yang ada.

![Screenshot 2025-01-02 111417](https://github.com/user-attachments/assets/f77a1940-ea9c-4808-91c9-098ede4e3039)




## KESIMPULAN
Program ini merupakan aplikasi sederhana untuk memvalidasi data pendaftaran pengguna dengan memeriksa format nama lengkap, nomor telepon, dan email. Validasi dilakukan menggunakan regular expression dan metode bawaan Python untuk memastikan nama hanya berisi huruf dan spasi, nomor telepon hanya terdiri dari angka, serta email mengandung karakter @ dan . sebagai tanda dasar format yang benar. Jika data yang dimasukkan tidak memenuhi kriteria, program akan memberikan pesan kesalahan yang spesifik untuk setiap input. Meskipun efektif untuk validasi dasar, program ini dapat ditingkatkan dengan validasi yang lebih ketat, seperti memeriksa struktur lengkap email, panjang nomor telepon, atau dukungan untuk karakter khusus pada nama. Program ini cocok sebagai pondasi awal untuk aplikasi pendaftaran yang lebih kompleks.
