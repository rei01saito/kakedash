# Kakedash

駆け出しエンジニアのためのスキル管理アプリ。

### 機能

- 現在の自身のエンジニアレベルを可視化する
  - 何が足りてないか把握する

#### 環境構築

1. 環境変数関連のファイルをコピーします

```
$ cp back/.env.sample back/.env
$ cp db/.env.sample db/.env
$ cp db/password.txt.sample db/password.txt
$ cp front/.env.sample front/.env
```
2. コンテナを起動します

```
$ docker-compose up -d
```

3. 各サービスへアクセスします

バックエンド|フロントエンド
:-:|:-:
localhost:3000 | localhost:8080
