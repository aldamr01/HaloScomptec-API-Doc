# Sistem Informasi Android "Halo SCOMPTEC"

<p align="center">
  <img width="250" src="images/logo.png" text="Logo of SCOMPTEC">
</p>

|Task Name|Description|
|:---|:---|
|`Tables Release`|1.0 |
|`Document Status`|DRAFT |
|`Document Owner`|[Aldion Ammirrul Endryanto](https://www.instagram.com/aldamr01)|
|`UI/UX Designer`|[Aditya Nanda Utama](https://www.instagram.com/adit.nanda)|
|`Android Developer`|[Aditya Nanda Utama](https://www.instagram.com/adit.nanda)|
|`Web Developer`|[Aldion Ammirrul Endryanto](https://www.instagram.com/aldamr01)|
|`Database Designer`|[Aldion Ammirrul Endryanto](https://www.instagram.com/aldamr01)|

## Background
<p align="justify">
Perkembangan teknologi saat ini semakin pesat. Tidak dapat dipungkiri bahwasanya semua elemen sudah terjangkit dengan adanya teknologi. Teknologi saat ini yang sedang menjadi trend yaitu teknologi mobile, terutama Android. Dikarenakan pada zaman sekarang untuk saling terhubung tidak dibatasi tempat dan waktu. Dengan adanya versi mobile user dapat menggunakan teknologi dimanapun dan kapanpun. Sehingga teknologi ini sudah menjadi kebutuhan sehari-hari. Oleh karena itu kami membuat aplikasi android bernama "Halo SCOMPTEC" yang bertujuan untuk mempermudah proses bisnis yang berada di SCOMPTEC.
</p>

## Requirements
|No.|User Story Title|User Story Description|Priority|Notes|
|:---|:---|:---|:---|:---|
|`1`|Registrasi Akun|<p align="justify">Pengguna sebagai calon pendaftar kursus maupun sudah mendaftar kursus di layanan kursus SCOMPTEC</p>|Must have|Akun terdaftar dapat berupa alamat email|
|`2`|Integrasi Email|<p align="justify">Ketika pengguna lupa kata sandi untuk login, mereka dapat menerima password baru melalui email.</p>|Must have|Pengguna harus memasukkan alamat email yang benar di aplikasi|
|`3`|Integrasi SMS|<p align="justify">Ketika pengguna lupa kata sandi untuk login, mereka dapat menerima password baru melalui SMS.</p>|Optional|Pengguna harus memasukkan nomor telepon yang benar di aplikasi|
|`4`|API|<p align="justify">API (Application Programming Interface) dibutuhkan agar lalu lintas transaksi dalam aplikasi dapat berjalan dengan semestinya</p>|Should have|Web Developer membuat API agar transaksi dapat diakses oleh Android|

## API Documentation

Dokumentasi API terkait Aplikasi HaloScomptec

| NO | URL | METHOD | REQUEST | RESPONSE |
|----|-----|--------|---------|----------|
|1.  | /API/login | POST | username , password | kode , pesan , data |
|2.  | /API/register | POST | username , email , password , nama | kode , pesan |
|3.  | /aktivasi | POST | token | kode , pesan |
|4.  | /API/reset | POST | email | kode , pesan |
|5.  | /API/userinfo | PUT | id , token | kode , pesan , data |
|6.  | /API/update/text | POST | id,token | kode , pesan |
|7.  | /API/update/foto | POST | id,token,foto(image) | kode , pesan |
|8.  | /API/update/password | POST | id,token,password | kode , pesan |
|9.  | /API/kelembagaan/create | POST | token,judul,keterangan | kode , pesan |
|10. | /API/kelembagaan/update | POST | id,token,judul,keterangan | kode , pesan |
|11. | /API/kelembagaan/delete | POST | id,token | kode , pesan |
|12. | /API/kelembagaan/show | POST | token | kode , pesan , data |
|13. | /API/kelembagaan/find | POST | id,token | kode , pesan , data|
|14. | /API/struktur/create | POST | token,foto | kode , pesan |
|15. | /API/struktur/update | POST | id,token,foto | kode , pesan |
|16. | /API/struktur/delete | POST | id,token | kode , pesan |
|17. | /API/struktur/show | POST | token | kode , pesan , data |
|18. | /API/instruktur/create | POST | token,foto,nama,no_telepon,deskripsi | kode , pesan |
|19. | /API/instruktur/update | POST | id,token,foto,nama,no_telepon,deskripsi | kode , pesan |
|20. | /API/instruktur/delete | POST | id,token | kode , pesan |
|21. | /API/instruktur/show | POST | token | kode , pesan , data |
|22. | /API/pengumuman/create | POST | token,nama_pengumuman,isi,foto,id_akun | kode , pesan |
|23. | /API/pengumuman/update | POST | token,nama_pengumuman,isi,id | kode , pesan |
|24. | /API/pengumuman/delete | POST | token,id | kode , pesan |
|25. | /API/pengumuman/show | POST | token | kode , pesan , data |
|26. | /API/pengumuman/showByID | POST | token,id_akun | kode , pesan , data |
|27. | /API/pengumuman/find | POST | token,id | kode , pesan , data |
|28. | /API/pelatihan/create | POST | token,foto,nama,waktu_mulai,deskripsi,waktu_akhir,biaya,diskon,kapasitas,tipe | kode , pesan |
|29. | /API/pelatihan/update | POST | id,token,foto,nama,waktu_mulai,deskripsi,waktu_akhir,biaya,diskon,kapasitas,tipe | kode , pesan |
|30. | /API/pelatihan/delete | POST | id,token | kode , pesan |
|31. | /API/pelatihan/show | POST | token | kode , pesan , data |


## Daftar Akun
Akun untuk login ke Aplikasi Halo SCOMPTEC
1. Admin = username : admin , password : admin
2. Operator = username : operator , password : operator
3. User = username : adituser , password : 123456

## Changelog
Semua perubahan yang ada di aplikasi Android HaloScomptec akan di catat di bawah ini

## [Unreleased]

### [0.6.1] - 2019-03-24
#### Added
- Show pengumuman .
- Show daftar pelatihan .
- Show detail daftar pelatihan .
- Add icon keranjang .

### [0.5.1] - 2019-03-08
#### Added
- Insert daftar instruktur .
- Update daftar instruktur .
- Delete daftar instruktur .
- GET daftar instruktur .

### [0.4.1] - 2019-03-06
#### Added
- Insert data struktur organisasi .
- Update data struktur organisasi .
- Delete data struktur organisasi .
- GET data struktur organisasi .

#### Changed
- UI diperbarui .

### [0.3.1] - 2019-02-26
#### Added
- Insert data kelembagaan .
- Update data kelembagaan .
- Delete data kelembagaan .
- Cari & GET data kelembagaan .

### [0.2.1] - 2019-02-20
#### Added
- Reset Password .
- Ubah informasi user .
- Splash Screen .

#### Changed
- Informasi terkait perubahan password & Registrasi dikirim melalui Email .
- Get Data User & Ubah informasi memakai Token .
- Tampilan login .

### [0.0.1] - 2019-02-06
#### Added
- Registrasi user.
- Login user.
- Ganti password .
- Ambil data user .
