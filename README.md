# Nuxt.js project

## Build Setup

```
# コンテナ作成
$ docker-compose up -d

# app コンテナの中に入る
$ docker-compose exec app /bin/bash

# VSCodeにDockerのプラグインを入れている場合は
# attach shell でコンテナの中に入れる。

# コンテナの中に入ったら、
# 初回だけ、パッケージインストール
$ yarn install
$ cd server
$ yarn install
$ cd /app

# 初回だけ、envファイルのコピー
$ cp /app/server/.env.example /app/server/.env
$ cp /app/server/prisma/.env.example /app/server/prisma/.env

# 開発用のサーバー起動 http://localhost でブラウザからアクセスできる
$ yarn dev

# 本番用のビルドとサーバーの起動
$ yarn build
$ yarn start
```
