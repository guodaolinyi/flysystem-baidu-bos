# laravel-flysystem-bos
Laravel Flysystem adapter for Baidu Bos

##  Usage
config/filesystems.php

```
'bos' => [
    'driver' => 'bos',
    'bucket' => env('BAIDU_BOS_BUCKET'),
    'prefix' => env('BOS_PREFIX', 'bos'),
    'expire' => -1,
    'options' => [
        'credentials' => [
        'accessKeyId' => env('BAIDU_ACCESS_KEY_ID'),
        'secretAccessKey' => env('BAIDU_SECRET_ACCESS_KEY')
    ],
    'endpoint' => env('BAIDU_ENDPOINT'),
    'protocol' => 'https',
    ]
],
```



