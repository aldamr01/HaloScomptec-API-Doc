<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>


## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).


# API Documentation

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

# Daftar Akun
Akun untuk login ke Aplikasi Halo SCOMPTEC
1. Admin = username : admin , password : admin
2. Operator = username : operator , password : operator
3. User = username : adituser , password : 123456

# Changelog
Semua perubahan yang ada di aplikasi Android HaloScomptec akan di catat di bawah ini

## [Unreleased]

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
