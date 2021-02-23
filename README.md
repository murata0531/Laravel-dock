# docker-laravel

コンテナ作成

```
$ docker-compose up -d --build
```

コンテナ破棄

```
$ docker-compose down --rmi all --volumes --remove-orphans
```

各種コンテナに入る

```
appコンテナ：ここでlaravelやphpなどを動かしている
$ docker-compose exec app bash
```

```
dbコンテナ：ここでmysqlを動かしている
$ docker-compose exec db bash
```

```
webコンテナ：ここでnginxを動かしている
$ docker-compose exec web bash
```

構築

```
$ docker-compose exec app bash
```

```
bash# cp .env.example .env
```

```
bash# composer install

bash# npm install && npm run dev

bash# php artisan key:generate
```
