# Easyly PHP Library


![npm](https://img.shields.io/npm/v/easyly)
![NPM](https://img.shields.io/npm/l/easyly)

## Composer

You can install the bindings via [Composer](http://getcomposer.org/). Run the following command:

```bash
composer require easyly/easyly-php
```


To use the bindings, use Composer's [autoload](https://getcomposer.org/doc/01-basic-usage.md#autoloading):

```php
require_once 'vendor/autoload.php';
```

## Manual Installation

If you do not wish to use Composer, you can download the [latest release](https://github.com/Easyly-io/easyly-php/releases). Then, to use the bindings, include the `init.php` file.

```php
require_once '/path/to/easyly-php/init.php';
```


## Getting Started

Simple usage looks like:

```php
$easyly = new \Easyly\EasylyClient('sk_test_XXX....');
$lead = $easyly->leads->create([
    'name' => 'john doe',
    'email' => 'john@example.com'
]);
echo $lead->id;
```


### Full documentation can be found on the [Easyly Documentation](https://api.easyly.com)

### Contributing

If you would like to contribute to Easyly, please make sure to read our
[contributor guidelines](CONTRIBUTING.md).