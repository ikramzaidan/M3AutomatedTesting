# PERHATIKAN BAIK-BAIK!!!

# REQUIREMENT MODUL 3
Halo teman-teman, selamat datang di modul 3 dari praktikum Perancangan Perangkat Lunak EAD laboratory 2024, kali ini teman-teman akan melakukan automated testing pada aplikasi laravel yang sudah dibuat. Hal pertama yang perlu dilakukan ketika ingin menjalankan project ini, pastikan teman-teman memiliki requirement sebagai berikut :

- PHP >= 8.0
- Composer
- Node.js (https://nodejs.org/en)
- mysql
- Google Chrome

## Pastikan semua requirement di atas sudah terinstall pada laptop masing-masing! Browser yang digunakan untuk melalukan testing ini wajib menggunakan `Google Chrome`.

jika sudah memenuhi kriteria diatas teman-teman bisa melakukan clone pada project ini dan menjalankannya. caranya sebagai berikut :

1. Lakukan clone proyek pada device kalian masing masing `git clone <link repository>` 

2. `composer install`

### NOTE: Jika terjadi error pada saat menjalankan `composer install` atau `composer require laravel/dusk --dev`, pastikan extensi zip pada PHP sudah diaktifkan. Caranya jalankan perintah `php --ini` pada terminal di vscode, lalu buka direktori file `php.ini` yang muncul dengan cara tahan `CRTL` lalu klik direktorinya. Kemudian cari kata kunci `zip` sampai ketemu `;extension=zip`, hilangkan tanda `;` lalu save file tersebut. Jalankan kembali perintah installasinya.

3. `npm install` Pastikan Node.js sudah terinstall pada perangkat kalian

4. `cp .env.example .env`

### NOTE: Jika tidak bisa, ganti perintah `cp` menjadi `copy`

5. Generate key dengan perintah `php artisan key:generate`

6. `composer require laravel/dusk --dev`

7. `php artisan dusk:install`

8. `php artisan dusk:chrome-driver`

9. Migrate database dengan perintah 
`php artisan migrate`

10. Jalankan aplikasi dengan perintah 
`php artisan serve`
`npm run dev`

11. Sesuaikan variabel `APP_URL` di file `.env` dengan port server kalian (contoh: http://localhost:8000)

Selamat mengerjakan ya :)
