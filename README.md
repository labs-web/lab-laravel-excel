<=================== How to intsall package Excel Maatwebsite\Excel ======================> 



1- install laravel project ==> composer create-project laravel/laravel [name project]

2- Edit in file php.ini ===> make extension=gd enabled

3- install package ====> composer require maatwebsite/excel:*

4- then Go to composer.json and update ===> "maatwebsite/excel": "*" to "maatwebsite/excel": "3.1.48"

5- composer update

6- Go to config->app.php :
    add to providers ===> Maatwebsite\Excel\ExcelServiceProvider::class,
    Add to aliases 'Excel' =>Maatwebsite\Excel\Facades\Excel::class,

7- composer dump-autoload

8- Run this command  php artisan vendor:publish --provider="Maatwebsite\Excel\ExcelServiceProvider" --tag=config








