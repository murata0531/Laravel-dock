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
