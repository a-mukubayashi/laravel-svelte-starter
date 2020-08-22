# laravel-svelte-starter

- PHP 7.2
- Laravel 7.24
- svelte 3.0
- typescript 3.9.3

## set environment
./docker/.env
```
COMPOSE_PROJECT_NAME=laravel-svelte
MYSQL_ROOT_PASSWORD=
MYSQL_USER=
MYSQL_PASSWORD=
```

## docker setup
```
docker-compose build
docker-compose up -d

# larvel
docker exec -it laravel-svelte-backend bash
cd app
composer install

# svelte
docker exec -it laravel-svelte-client bash
cd app
yarn
```
## Laravel start
see: http://localhost/api/sample/hello

## svelte start
```
docker exec -it laravel-svelte-client bash -c "cd /opt/src/app && yarn build -w"
```
see: http://localhost/#/
