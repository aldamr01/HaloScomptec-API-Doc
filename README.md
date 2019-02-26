<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>


## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).


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
