## Dockerでの開発環境を構築した
<p>使用PC MacBook M2</p>

## 使用技術
<ol>
    <ul>PHP8.1</ul>
    <ul>MYSQL</ul>
    <ul>MYSQLAdmin</ul>
</ol>

## 使用コマンド

### 立ち上げ

docker-compose.ymlファイルが存在する場所にいき、コマンドを叩く。

```
$ docker compose up
```

### 　PHPコンテナに中入る

```
$ docker compose exec php bash
```

### Mysqlコンテナに入る

```
$ docker exec -it mysql bash
```

```
$ mysql -u [DBユーザー名] -p
```