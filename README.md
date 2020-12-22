"generate laravel project with docker :"

- php
- mysql
- redis
- node
- composer
- nginx

```
step 0:
git clone git@github.com:okirim/generate-laravel-stack-with-docker.git


step 1: create laravel project
docker-compose run --rm composer create-project laravel/laravel . --prefer-dist


step 2:  run nginx server (http://localhost:8000)
docker-compose up --rm -d server


step 3:  replace the .env file
mv docker.env ./laravel/.env


- use composer 
install php package with composer example :
docker run --rm  composer require firebase/php-jwt

-use npm
install npm packages with node example :
docker run --rm -v npm install nodemon

-use artisan example:
docker run --rm artisan make:model Post
```