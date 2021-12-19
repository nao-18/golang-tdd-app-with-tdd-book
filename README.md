# golang-tdd-app-with-tdd-book

## dockerコマンド
---

### コンテナ作成
~~~bash
$ docker-compose build
~~~

### コンテナ実行(バックグラウンド)
~~~bash
$ docker-compose up -d
~~~

### コンテナへ入る
~~~bash
$ docker-compose exec -it コンテナ名(app) sh
~~~

### 依存解決
~~~bash
$ docker-compose run --rm app go mod tidy
~~~

## テスト
---

### テスト実行
~~~bash
$ docker-compose run --rm app go test
~~~

### カレントディレクトリ以下の全てのテストを再帰的に実行
~~~bash
$ docker-compose run --rm go test ./... -v
~~~

