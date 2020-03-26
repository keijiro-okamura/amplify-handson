# amplify-handson
AWS Amplify Hands-on

# install
```shell script
$ git clone git@github.com:keijiro-okamura/amplify-handson.git
$ cd amplify-handson
$ docker-compose up -d
```

## npm ビルドインサーバ起動
```shell script
# ローカル
# コンテナが起動していることを確認
$ docker ps
# コンテナ内に移動
$ docker exec -it amplify_handson_container /bin/bash

#ここからコンテナ内
$ cd myamplifyproject
$ npm run serve
```
これで`http://localhost:8080/`にアクセスしてVueのWelcomeページが表示されたら環境構築は完了です。

## dockerコンテナ削除
```shell script
$ docker stop amplify_handson_container
```