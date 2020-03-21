# opcache-config-for-dev-sample

開発環境向けOpcache設定のサンプルです。

```shell
git clone git@github.com:tenkoma/opcache-config-for-dev-sample.git
cd opcache-config-for-dev-sample
cp .env.example
docker-compose run composer composer install
docker-compose up -d
docker-compose exec php-fpm php artisan key:generate
```
