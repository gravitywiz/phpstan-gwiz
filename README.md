# `gravitywiz/phpstan-gwiz` [![Packagist Version](https://img.shields.io/packagist/v/gravitywiz/phpstan-gwiz)](https://packagist.org/packages/gravitywiz/phpstan-gwiz) 

A PHPStan extension for Gravity Forms and WooCommerce. It adds type aliases for Gravity Forms and WooCommerce.
Additionally, there are other various config changes to ignore errors, etc.

# Usage

Add to your Composer project that is already using PHPStan. This package is compatible with `phpstan/extension-installer`
so nothing outside of `composer require --dev "gravitywiz/phpstan"` is needed.

If you're not using `phpstan/extension-installer`, the files can be added to your `phpstan.neon` file manually by
adding them to `includes` like so:

```neon
parameters:
    includes:
        - ./vendor/gravitywiz/phpstan/gravityforms.neon
        - ./vendor/gravitywiz/phpstan/woocommerce.neon
```