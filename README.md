# 環境構築（Rails + Docker)
下記の課題対応レポジトリになります。


07_docker/003_docker.md (dockerで開発構築を構築する より)
https://github.com/happiness-chain/practice/blob/main/07_docker/003_docker.md

## 手順を記載

- ①当リポジトリをcloneする
```
git clone git@github.com:Taguchi-ivi/rails-docker.git
```

- ②フォルダへ移動
```
cd rails-docker
```

- ③dockerを起動する(dockerのインストールは省略)
```
docker-compose up -d
```

- ④dbを作成
```
docker-compose run web rails db:create
```

- ⑤dbを更新
```
docker-compose run web rails db:migrate
```

- ⑥確認
全ての操作が完了したので下記をクリックしサイトが表示されるか確認する

    http://localhost:3000
