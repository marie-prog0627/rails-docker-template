## initialize

1. docker-compose run web rails new . --force --database=postgresql
2. docker-compose build
3. config/database.ymlのdefaultに、username: 'admin' / password: 'admin-pass'を追加

## when start
1. docker-compose up -d
2. docker-compose run web bundle exec rails db:create
3. localhost:3000にアクセス

## when close
1. docker-compose down
