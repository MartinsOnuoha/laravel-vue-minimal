<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/MartinsOnuoha/laravel-vue-minimal/master/public/logo.png" width="200"></a></p>

## Laravel-Vue-Minimal

Get started quickly with Vue, Vuex, Vue-Router in Laravel.

## Setup

### Clone the repository

```bash
git clone https://github.com/MartinsOnuoha/laravel-vue-minimal.git
```

### Install Dependencies

```bash
yarn && composer install
```

### Copy .env

```bash
cp .env.example .env
```

### Generate App Key

```bash
php artisan key:generate
```

### Start Server

```bash
php artisan serve
```

```bash
yarn run watch
```

## Project Structure

### Vue

You can find the Vue app structure under `resources/js`

```tree
📁 Components
📁 Mixins
📁 Pages
📁 Router
📁 Store
📁 Styles
  🗳 App.vue
  🗳 App.js
```

## Docker

This project uses [Sail](https://laravel.com/docs/9.x/sail) to run the app within a docker environment. If you would like to run the project within a docker container you can do this by first building the container and then running it.

Within the project directory run:

```bash
docker-compose build
```

After the build is complete you can start the container by running:

```bash
docker-compose up
```

Alternatively if you have composer installed correclty and the composer command is available, then you can run:

```bash
composer run-script sail
```

You should find the app running in any port value set for `APP_PORT` in `.env`.
