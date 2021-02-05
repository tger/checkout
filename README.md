# Laravel Package for handling Checkout used in Ecommerce packages

[![Latest Version on Packagist](https://img.shields.io/packagist/v/tipoff/checkout.svg?style=flat-square)](https://packagist.org/packages/tipoff/checkout)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/tipoff/checkout/run-tests?label=tests)](https://github.com/tipoff/checkout/actions?query=workflow%3ATests+branch%3Amaster)
[![Total Downloads](https://img.shields.io/packagist/dt/tipoff/checkout.svg?style=flat-square)](https://packagist.org/packages/tipoff/checkout)

## Installation

You can install the package via composer:

```bash
composer require tipoff/checkout
```

The migrations will run from the package. You can extend the Models from the package if you need additional classes or functions added to them.

You can publish the config file with:
```bash
php artisan vendor:publish --provider="Tipoff\Checkout\CheckoutServiceProvider" --tag="checkout-config"
```

#### Registering the Nova resources

If you would like to use the Nova resources included with this package, you need to register it manually in your `NovaServiceProvider` in the `boot` method.

```php
Nova::resources([
    // TBD
]);
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](.github/CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [Tipoff](https://github.com/tipoff)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.