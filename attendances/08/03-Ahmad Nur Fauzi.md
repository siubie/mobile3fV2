Rangkuman Minggu ke-8

Project Menggunakan Laravel API
- Mempelajari cara membuat project laravel menggunakan API
- Mempelajari cara membuat database pada project laravel tepatnya difile .env
- Mempelajari cara membuat category yaitu index,store,show,update,destroy
- Mempelajari cara migration tabel
- Membuat controller API dengan perintah diterminal yaitu php artisan make:controller CategoryController --api-
- Penggunaan aplikasi postman sebagai isi data, dan methodnya seperti contoh GET,PUT,DELETE,POST

Langkah-Langkah membuat API pada Laravel

1. Membuat database dan mengkoneksikan di file .env pada project laravel
2. Membuat model yaitu model category
3. Membuat file migration, dimana terdapat table id,nama,timestamp, setelah selesai data tersebut akan dimasukan kedalam Database dengan perintah php artisan migrate
4. Membuat Controller yaitu CategoryController yang dimana terdapat 5 function index,show,update,dan destroy
   Kita juga dapat membuat folder request untuk meletakkan rules atau validated yang diperlukan di sebuah controller
5. Setting pada routes api.php supaya bisa memanggil Controller yang diperlukan
