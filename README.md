<p><a href="https://www.buymeacoffee.com/ardean"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="ardean" /></a><a href="https://ko-fi.com/ardean"> <img align="left" src="https://cdn.ko-fi.com/cdn/kofi3.png?v=3" height="50" width="210" alt="ardean" /></a></p><br><br>

# TMAIL - Multi Domain Temporary Email System

Sistem penerima email sementara multi-domain. Dibuat menggunakan Laravel.

# Requirements

## Server Requirements
- PHP >= 8.1
- MySQL >= 5.6
- OpenSSL PHP Extension
- PDO PHP Extension
- Mbstring PHP Extension
- Tokenizer PHP Extension
- XML PHP Extension
- Ctype PHP Extension
- JSON PHP Extension
- BCMath PHP Extension
- IMAP PHP Extension
- iconv PHP Extension
- ZIP PHP Extension
- Fileinfo PHP Extension
- Set allow_url_fopen = ON
- Email with IMAP Support
- Default Email Forwarder (Catch all Email)
- IMAP search ability
- Everything which requires Laravel 8 to run
- Enabled symlink function

# Installasi

Berikut adalah langkah-langkah dengan tangkapan layar cPanel yang merupakan salah satu panel kontrol hosting terpopuler. Namun, langkah-langkah ini dapat ditransfer ke panel kontrol mana pun yang Anda gunakan.

## Unggah File
- Buka zip file yang Anda unduh dari CodeCanyon.
- Anda akan menemukan nama file Files.zip
- Unggah file itu di File Manager dan Unzip
![Screenshot](https://i.imgur.com/E9Yw34v.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/file_manager_upload.png)

![Screnshot](https://docs.tmail.thehp.in/assets/images/file_extract.png)

## Buat Database dan User

- Buka Database MySQL atau Wizard
- Buat Basis Data MySQL
- Buat Nama Pengguna dan Kata Sandi MySQL
- Catat rincian ini di Notepad karena kita harus memasukkannya ke dalam - Penginstal TMail
- Tetapkan Pengguna ke Database MySQL dengan semua izin

![Screenshot](https://docs.tmail.thehp.in/assets/images/mysql_wizard.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/create_database.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/create_database_user.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/assign_database_permissions.png)

## Buat Akun Email

- Buka Akun Email
- Buat ID Email dan atur Kata Sandi
- Catat detail ini di Notepad karena kita harus memasukkannya di TMail Installer
- Siapkan catch-all untuk meneruskan semua email dari domain tersebut ke ID Email yang dibuat di atas

![Screenshot](https://docs.tmail.thehp.in/assets/images/email_accounts.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/create_email_account.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/default_address.png)

![Screenshot](https://docs.tmail.thehp.in/assets/images/setup_catch_all.png)

## Masuk ke Penginstall Tmail

Saatnya memuat Penginstal TMail. Cukup navigasikan ke situs web Anda di mana penginstal akan dimuat secara otomatis untuk Anda.

## Database detail

Di sini Anda akan memasukkan Nama Database, Pengguna, Kata Sandi, Host dan Port. Anda dapat mempertahankan host dan port apa adanya jika server Anda mengizinkan penggunaan localhost sebagai nama host dan MySQL berfungsi pada port 3306.

![Screenshot](https://docs.tmail.thehp.in/assets/images/tmail_database.png)

## Detail Lisensi

Masukan nama acak, karena ini adalaah versi demo yang kami buat untuk penggunaan gratis.

## Detail IMAP

Anda harus memasukkan kredensial akun Email yang Anda buat pada langkah sebelumnya.

![Screenshot](https://docs.tmail.thehp.in/assets/images/tmail_imap.png)

## Buat Akun Admin

Langkah terakhir adalah membuat akun Admin agar Anda dapat mengelola TMail Anda.

![Screenshot](https://docs.tmail.thehp.in/assets/images/tmail_admin.png)
# Referensi API

Untuk semua ahli teknologi di luar sana, TMail juga menawarkan API sehingga Anda dapat membuat Aplikasi sendiri dengan menggunakannya.

Untuk menggunakan API, Anda perlu membuat Kunci API dengan masuk ke Panel Admin TMail -> Pengaturan -> Lanjutan (bagian). Anda dapat membuat beberapa Kunci API.

## Daftar Domain

Dapatkan daftar domain yang tersedia saat ini.

`Get`
```
https://yourdomain.com/api/domains/[apikey]

```
## Parameter

[apikey] - Kunci yang mungkin telah Anda atur di Panel Admin TMail Anda.
## Buat Email

Validasi ID Email dan berikan yang sudah dibersihkan.

`Get`
```
https://yourdomain.com/api/email/[email]/[apikey]

```

## Parameter

[apikey] - Key which you may have set in your Admin Panel of TMail.

[email] - Email ID that you want to create.
## Ambil Pesan

Dapatkan pesan email dari ID Email yang diberikan.

`Get`
```
https://yourdomain.com/api/messages/[email]/[apikey]

```

## Parameter

[apikey] - Key which you may have set in your Admin Panel of TMail.

[email] - Email ID that you want to create.

## Hapus Pesan

Hapus pesan email tertentu dengan ID yang diberikan.

`Get`
```
https://yourdomain.com/api/message/[message_id]/[apikey]

```

## Paramenter

[apikey] - Key which you may have set in your Admin Panel of TMail.

[message_id] - Unique identifier for the specific message to delete.
# Credit

Fonts:

- Poppins Font Face - https://fonts.google.com
- Icons Font Face - https://fontawesome.com/

Scripts:

- Laravel Framework by Taylor Otwell (License: MIT) - https://laravel.com
- Laravel Jetstream (License: MIT)https://github.com/laravel/jetstream
- IMAP Library for Laravel (License: MIT) - https://github.com/ddeboer/imap
- Tailwind by twbs (License: MIT) - https://github.com/tailwindlabs/tailwindcss
- Alpine JS (License: MIT) - https://github.com/alpinejs/alpine

Images:

- Freepik - https://freepik.com/
