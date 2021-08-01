# Dockerized Laravel 8 & Vue 3 App with TypeScript

Docker development implementation for Laravel 8.\* with:

- Nginx
- PostgreSQL
- PHP8.0
- Vue
- Node

## Installation

- Clone this repository `git clone git@github.com:sadhakbj/Laravel-8-vue3-typescript.git`
- Make sure you have docker installed on your local machine, you do not need to have php / mysql / redis / node installed on your machine
- Copy `.env` file: `cp .env.example .env`
- Set the environment variables in `.env` file
- Run command: `docker-compose up --build -d`
-  Run the container in bash mode: `docker exec -it Laravel_php /bin/sh`
- Inside this container now you can run all the commands as if if you are on local environment:
- Install composer dependencies: `composer install`
- Generate key: `php artisan key:generate`
- Run migration: `php artisan migrate`
- Run seeder: `php artisan db:seed`
- Install javascript dependencies: `yarn`
- Compile the assets: `yarn dev` / `yarn watch`  
- You can access the project at: `http://localhost:8000`


