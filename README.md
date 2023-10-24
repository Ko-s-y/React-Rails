### Rails API
```
docker-compose run api rails new . --force --no-deps -d mysql --api
```

### Gemfile更新の際の再ビルド
```
docker-compose build
```

### データベースの作成
```
docker-compose run api rails db:create
```

### backend webserver立ち上げ
```
docker-compose up -d
```

### テストAPIの呼び出し
```
curl http://localhost:3001/api/v1/test
```
