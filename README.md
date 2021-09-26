## Docker LEMP環境テンプレート(Linux + Nginx + MySQL + PHP)

### 初回pull時

```
$ docker-compose build --no-cache
```

### Build後のコンテナ起動

```
$ docker-compose up -d
```

### Laravel環境準備

```
$ docker-compose exec php bash
$ cp .env.example .env
$ composer install
$ php artisan key:generate
$ php artisan migrate
```



**下記にアクセス**

http://localhost:8000/
