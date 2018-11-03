#Upload  1.0.0
This is based on datatables 

Add to your composer.json
 "repositories": [
        {
            "type": "path",
            "url": "packages/mjvamorim/upload",
            "options": {
                "symlink": true
            }
        },

cd packages/mjvamorim

git clone https://github.com/mjvamorim/upload.git

cd ../..

composer require mjvamorim/upload

Add in your config/app.php

    Amorim\Upload\UploadServiceProvider::class,
       

composer update

php artisan vendor:publish --provider="Amorim\Upload\UploadServiceProvider" --tag=assets

php artisan migrate



