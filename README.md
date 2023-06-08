## Laravel, Chatify, dan Pusher

### Fitur

-   Tampilan chat real-time yang responsif.
-   Kemampuan untuk mengirim dan menerima pesan secara instan.
-   Pengguna dapat melihat riwayat pesan sebelumnya.
-   Dibangun menggunakan teknologi Laravel, Chatify, dan Pusher yang populer.

### Preview

Darkmode/Lightmode

![Darkmode](https://raw.githubusercontent.com/rakarmp/chatify/master/preview/21.PNG)

![Lightmode](https://raw.githubusercontent.com/rakarmp/chatify/master/preview/22.PNG)

### Cara Menggunakan

1.  Pastikan Anda memiliki akun Pusher. Jika belum, daftar dan buat aplikasi baru di [https://pusher.com](https://pusher.com/).
2.  Clone repositori ini ke direktori lokal Anda:

```shell
git clone https://github.com/rakarmp/chatify
```

3.  Navigasikan ke direktori proyek:

```shell
cd chatify
```

4.  Instal paket-paket yang diperlukan dengan menjalankan perintah berikut:

```shell
composer install

npm install
```

5.  Salin file `.env.example` ke `.env`:

```shell
cp .env.example .env
```

6.  Buka file `.env` dan ubah konfigurasi database sesuai dengan lingkungan Anda.
7.  Atur konfigurasi Pusher di file `.env` dengan informasi yang Anda peroleh saat membuat aplikasi Pusher:

`BROADCAST_DRIVER=pusher
PUSHER_APP_ID=YOUR_APP_ID
PUSHER_APP_KEY=YOUR_APP_KEY
PUSHER_APP_SECRET=YOUR_APP_SECRET
PUSHER_APP_CLUSTER=YOUR_APP_CLUSTER`

Pastikan untuk mengganti `YOUR_APP_ID`, `YOUR_APP_KEY`, `YOUR_APP_SECRET`, dan `YOUR_APP_CLUSTER` dengan nilai yang sesuai.

8.  Generate key aplikasi Laravel dengan menjalankan perintah berikut:

```shell
php artisan key:generate
```

9.  Jalankan migrasi untuk membuat tabel pesan di database:

```shell
php artisan migrate
```

10. Jalankan server lokal untuk menjalankan aplikasi:

```shell
php artisan serve
```

11. Buka aplikasi di browser Anda dengan mengunjungi URL [http://localhost:8000](http://localhost:8000/).

12. Anda dapat mulai mengirim dan menerima pesan secara real-time dengan menggunakan fitur chat yang disediakan.

### Kontribusi

Jika Anda ingin berkontribusi pada proyek ini, silakan fork repositori ini dan buat branch baru untuk setiap fitur atau perbaikan yang Anda kerjakan. Setelah selesai, ajukan pull request ke branch utama.
