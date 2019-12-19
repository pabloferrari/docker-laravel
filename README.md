# docker-laravel

1. - Copy these files to the root of your project

2. - If you need install packages

$ docker run --rm -v $(pwd):/app composer install

3. - Permissions

$ sudo chown -R $USER:$USER ~/your-project

4. - Copy .env (if it doesn't exist)

$ cp .env.example .env

5. - Build containers

$ docker-compose up -d

5. ~ See containers

$ docker ps

6. - KEY:GENERATE
$ docker-compose exec app php artisan key:generate
* app: name of container

7. - CONFIG:CACHE
$ docker-compose exec app php artisan config:cache
* app: name of container

8. - PHP ARTISAN MIGRATE
$ docker-compose exec app php artisan migrate / php artisan migrate --seed
* app: name of container

------------------------------------------------------------------------------------

EXEC containers

$ docker-compose up -d