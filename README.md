# docker で nuxt.js 開発環境

## 参考url

[docker で nuxt.js を開発環境をたてるだけ : Qiita](https://qiita.com/kitsuki00/items/ed51dbb254bcc6c94fbd)

[NUXTJS](https://ja.nuxtjs.org/)

## コマンド

 dockerimage 作成 

```shell
docker-compose build 
```

コンテナ内のコマンドをexec使わず叩く
(docker-compose run --rm <サービス名(nuxt)> <コマンド>)
```shell
docker-compose run --rm nuxt npx create-nuxt-app nuxt_project
```
コンテナ立ち上げ
```shell
docker-compose up -d
```
コンテナ起動確認
```shell
docker-compose ps
```
コンテナ内に入る

```
docker exec -it nuxtjs /bin/sh

cd nuxt_project　// ディレクトリ移動

npm run dev //実行

localhost:3000 // ブラウザでひらく

ctrl + c で終了

exit 　// コンテナから出る
```

コンテナ　終了
```shell
docker-compose stop
```

コンテナ削除
```shell
docker-compose down
```

