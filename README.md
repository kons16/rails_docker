# Rails + Docker
既存のRailsアプリ(MySQL)をDockerに乗せてみたサンプルです。  

## 使い方
1. `config/database.yml`のパスワードと`docker-compose.yml`の`MYSQL_ROOT_PASSWORD=XXX`を一致させる。
1. `$ docker-compose build`
1. `$ docker-compose up` でサーバーが立ち上がります。
1. 別タブで`$ docker-compose run web rails db:create`でDBを作る。
1. `http://127.0.0.1:3000/`にアクセスしてページが見れるか確認。
