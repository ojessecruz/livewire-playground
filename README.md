# Livewire Playground

A sandbox project intended solely for testing and experimenting with Laravel and Livewire, using Laravel Sail as the development environment.

## Stack

| Package            | Version  |
|--------------------|----------|
| PHP                | 8.3      |
| Laravel Framework  | 12.52.0  |
| Livewire           | 3.7.10   |
| MySQL              | 8.4      |

## Getting Started

### Prerequisites

- Docker Desktop

### Setup

```bash
composer install
cp .env.example .env
php artisan key:generate
```

### Running

```bash
./vendor/bin/sail up -d
./vendor/bin/sail artisan migrate
./vendor/bin/sail npm run dev
```

The application will be available at **http://localhost**.

### Stopping

```bash
./vendor/bin/sail down
```

## Useful Commands

```bash
# Artisan commands
./vendor/bin/sail artisan make:livewire ComponentName

# Composer
./vendor/bin/sail composer require package/name

# NPM
./vendor/bin/sail npm install
./vendor/bin/sail npm run build

# Shell access
./vendor/bin/sail shell

# MySQL CLI
./vendor/bin/sail mysql
```
