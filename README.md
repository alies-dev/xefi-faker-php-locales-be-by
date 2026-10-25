# Faker PHP — be_BY locale

Belarusian (`be_BY`) locale for [Faker PHP](https://github.com/xefi/faker-php).

> This package is a work in progress: no extension ships yet. Contributions are welcome.

## Installation

```bash
composer require --dev xefi/faker-php-locales-be-by
```

The service provider is discovered automatically through Composer.

## Usage

```php
use Xefi\Faker\Faker;

$faker = new Faker('be_BY');
```

Generators without a `be_BY` variant fall back to the default locale.

## Contributing

1. Fork the repository and create a branch from `main`.
2. Add an extension under `src/Extensions/` and register it in `FakerBeByServiceProvider::boot()`.
3. Add a test under `tests/Unit/`.
4. Run the suite with `vendor/bin/phpunit` (or `docker compose run php vendor/bin/phpunit`).
5. Open a pull request against `main`.

## License

MIT
