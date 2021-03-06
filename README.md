# Laravel docker base

LaravelアプリケーションをAWSへデプロイすることを想定したAmazonLinuxベースのLAMP開発環境。

# Containers

- Web
  nginx:latest
- App
  php8
- DB
  mysql:latest
- Mailhog
- Redis

# usage

```
git clone https://@github.com/IchikawaYoshihiro/laravel-docker-base.git
cd laravel-docker-base

cp .env.example .env

// create new Laravel application
laravel new src

docker-compose up -d
```
