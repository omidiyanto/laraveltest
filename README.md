# simple-docker-for-laravel
A pretty simplified Docker Compose workflow that sets up a local Laravel development

## Usage

To Start
- `docker-compose up -d`

To Stop
- `docker-compose down`

Three additional containers are included that handle Composer, NPM, and Artisan commands *without* having to have these platforms installed on your local computer. Use the following command examples from your project root, modifying them to fit your particular use case.

- `docker-compose run --rm composer update`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 
- `docker-compose run --rm php -v`

## Laravel Source Code

Put your laravel source code in src folder & configure .env file in your laravel project

1. Set mysql host to mysql
2. Set redis host to redis