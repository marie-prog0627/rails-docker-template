## initialize

1. docker-compose.ymlのwebとdbのvolumesの:前の相対パスを自分のカレントディレクトリの絶対パスに変更
2. docker-compose run web rails new . --force --database=postgresql
3. docker-compose build --no-cache
4. config/database.ymlのdefaultに、username: 'admin' / password: 'admin-pass'を追加

## when start
1. docker-compose up -d
2. docker-compose run web bundle exec rails db:create
3. localhost:3000にアクセス

## when close
1. docker-compose down

## when update
1. docker-compose build