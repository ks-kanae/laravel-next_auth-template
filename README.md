```
git clone ...
```
```
cd laravel-next_auth-template/laravel-next-app
```
.env.example を .env にコピーし、必要な値を設定
```
composer install
```
（Composer がない環境では、今回のように Docker 版 Composer を使う↓）
```
docker run --rm -u "$(id -u):$(id -g)" -v "$PWD":/app -w /app laravelsail/php82-composer:latest composer install
```
```
php artisan key:generate
```
```
./vendor/bin/sail up -d
```
```
cd ../next-frontend-app && npm install && npm run dev
```
