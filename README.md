# Lipsia Digital's WordPress plugin development PHPCS standard.

This is a superset of the [NeutronStandard](https://github.com/Automattic/phpcs-neutron-standard) and [PSR12](https://www.php-fig.org/psr/psr-12/) with some modifications.

## Installation

```sh
composer require --dev squizlabs/php_codesniffer dealerdirect/phpcodesniffer-composer-installer
composer require --dev lipsia/phpcs-wp-plugin-standard
```

## Usage

In your project's ruleset file, enable this ruleset by setting the `<rule>`.

```xml
<rule ref="LipsiaDigitalWordPressPlugin"/>
```
