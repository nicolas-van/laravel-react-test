# Laravel React Test

## Local Development

To install dependencies:

```
composer install
npm install
```

To compile JavaScript:

```
npm run dev
```

To run the web server:

```
php artisan serve
```

## Deployment on Heroku

After creating your application don't forget to configure your buildpacks:

```
heroku buildpacks:clean
heroku buildpacks:add heroku/php
heroku buildpacks:add heroku/nodejs
```

You must also configure some env parameters:

```
heroku config:set APP_KEY=$(php artisan --no-ansi key:generate --show)
heroku config:set APP_ENV=production
```
