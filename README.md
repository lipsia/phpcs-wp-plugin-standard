# Lipsia Digital's WordPress plugin development PHPCS standard.

This is a superset of the [NeutronStandard](https://github.com/Automattic/phpcs-neutron-standard) and [PSR12](https://www.php-fig.org/psr/psr-12/) with some modifications.

## Installation

```sh
composer require --dev squizlabs/php_codesniffer dealerdirect/phpcodesniffer-composer-installer
composer require --dev lipsia/phpcs-wp-plugin-standard
```

## Usage

In your project's ruleset file, enable this ruleset by setting the `<rule>` tag.

Minimal _phpcs.xml.dist_:

```xml
<?xml version="1.0"?>
<ruleset>
    <rule ref="LDWordPressPlugin"/>
</ruleset>
```

Or without a file:

```sh
./vendor/bin/phpcs --standard=LDWordPressPlugin .
```
