# web-application-from-docker-lecture

Udemy・米国AI開発者がゼロから教えるDocker講座の応用編第二弾のDocker compose を使って超本格Webアプリ開発環境の構築を実装する  
https://www.udemy.com/course/aidocker/learn/lecture/20295745#questions

## 構成

- Ruby on Rails
- Postgresql
- Travis CI
- Heroku


#### docker compose build

```
docker-compose build
```

#### docker-composeを使ってコンテナを立てる
```
docker-compose up -d
```

```
docker-compose ps
```

#### コンテナに入る
```
docker-compose exec web bash
```

#### コンテナ内でサーバーを立てる 
```
rails s -b 0.0.0.0
```





#### Dockerfileで作ったDocker imageをrunする方法

```
$ docker run -v ~/$pwd/product-register:/product-register -p 3000:3000 -it 4c1d8da98d2a bash
```

#### Docker-composeを使う時
- docker runが長くなる時
- 複数のコンテナを立ち上げるとき


#### docker-composeコマンド

```
docker-compose build(docker buildに対応)
docker-compose up(docker runに対応)
docker-compose ps(docker psに対応)
docker-compose exec <service>(docker execに対応)
docker-compose up--build(buildしてrun)
docker-compose down(stopしてrm)
```



## CICDパイプライン

#### Travis CI

#### Heroku



