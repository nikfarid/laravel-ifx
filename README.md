## Laravel Informix Database Package

Laravel-ifx is an Informix Database Driver package for [Laravel Framework](http://laravel.com/) - thanks @taylorotwell. Laravel-ifx is an extension of [Illuminate/Database](https://github.com/illuminate/database) that uses either the PDO extension wrapped into the PDO namespace.

**Please report any bugs you may find.**

- [Installation](#installation)
- [License](#license)

### Installation

Add `poyii/laravel-ifx` as a requirement to composer.json:

```terminal
$ composer require poyii/laravel-ifx
```

Skip below step if you are running Laravel newer than 5.6.

Once Composer has installed or updated your packages you need to register Informix DB. Open up `config/app.php` and find
the `providers` key and add:

```php
Poyii\Informix\InformixDBServiceProvider::class,
```

Finally you need to publish a configuration file by running the following Artisan command.

```terminal
$ php artisan vendor:publish --tag=config-informix
```

This will copy the configuration file to `config/informix.php`

### License

Licensed under the [MIT License](http://cheeaun.mit-license.org/).