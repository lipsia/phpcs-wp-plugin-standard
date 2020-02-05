# Lipsia Digital's WordPress plugin development standard

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

## Opinions

This ruleset is opinionated and that is a good thing.

### Rules that MUST NOT be changed

- main plugin file is in _./plugin.php_
- all other plugin files are autoloaded from _./src/_
- composer dependencies are in _./vendor/_
- convert tabs to 4 spaces

### Rules that CAN be changed

- use colors in report
- look into all files with extension _php_
- check 8 files in parallel
