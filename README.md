# Laravel Dusk Dashboard

A beautiful dashboard for your Dusk test suites.

[![Latest Version on Packagist](https://img.shields.io/packagist/v/Lubianfuchen/dusk-dashboard.svg?style=flat-square)](https://packagist.org/packages/Lubianfuchen/dusk-dashboard)
[![Quality Score](https://img.shields.io/scrutinizer/g/Lubianfuchen/dusk-dashboard.svg?style=flat-square)](https://scrutinizer-ci.com/g/Lubianfuchen/dusk-dashboard)
[![Total Downloads](https://img.shields.io/packagist/dt/Lubianfuchen/dusk-dashboard.svg?style=flat-square)](https://packagist.org/packages/Lubianfuchen/dusk-dashboard)

![](https://pociot.dev/storage/22/dusk-dashboard.gif)

## Installation

You can install the package via composer:

```bash
composer require Lubianfuchen/dusk-dashboard --dev
```

Next up, you need to go to your `DuskTestCase.php` that was installed by Laravel Dusk. You can find this file in your `tests` directory:

Find and replace this line:
```php
use Laravel\Dusk\TestCase as BaseTestCase;
```
with:
```php
use Lubianfuchen\DuskDashboard\Testing\TestCase as BaseTestCase;
```

## Usage

```
php artisan dusk:dashboard
```

Check out the documentation [here](https://pociot.dev/8-introducing-laravel-dusk-dashboard).

### Handling Asset Paths

Assets may not load or display properly when using relative paths due to port specification. Using Larvel's [Path Helpers](https://laravel.com/docs/5.7/helpers#available-methods) such as the `url()` and `asset()` helpers  (Ex: `{{ url('path/to/asset.css') }}`) will help overcome these pathing issues.

### Testing

``` bash
composer test
```

### Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

### Security

If you discover any security related issues, please email marcel@beyondco.de instead of using the issue tracker.

## Credits

- [Marcel Pociot](https://github.com/mpociot)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
