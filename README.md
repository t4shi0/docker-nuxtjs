# docker で nuxt.js を開発環境を建てる

## 参考url

[docker で nuxt.js を開発環境を建てるだけ : Qiita](https://qiita.com/kitsuki00/items/ed51dbb254bcc6c94fbd)

[NUXTJS](https://ja.nuxtjs.org/)

## コマンド

 dockerimage 作成 

```shell
docker-compose build 
```

コンテナ内のコマンドをexec使わず叩く
(docker-compose run --rm <コンテナ名> <コマンド>)
```shell
docker-compose run --rm nuxt npx create-nuxt-app 
```
コンテナ立ち上げ
```shell
docker-compose up -d
```
コンテナ起動確認
```shell
docker-compose ps
```
ブラウザ起動

localhost:8080

コンテナ　終了
```shell
docker-compose stop
```

コンテナ削除
```shell
docker-compose down
```

