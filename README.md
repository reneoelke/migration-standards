php-migration-standards
=======================

This composer _metapackage_ provides compatibility tests between any two of these PHP versions:
* PHP 4.4
* PHP 5.0
* PHP 5.1
* PHP 5.2
* PHP 5.3
* PHP 5.4
* PHP 5.5

Please refer to the single standard for detail.

!!! TODO link standards !!!

!!! TODO describe strategie for compatibility tests across multiple versions !!!

As with most phpcs standards a detailed report is generated.
Your code will not be modified.

install
-------

Git clone this repository and  the standards.

Either

```/bin/bash
git clone git@github.com:php-migrations/migration-standards.git
cd migrations-standards
composer install
```

Or add `php-migrations/standards` to the _require_/ _require-dev_ section of your `composer.json`.

usage
-----

Test compatibility between two versions like
```
./vendor/bin/phpcs --standard=PHP53to54 /path/to/your/code
```
And replace `PHP53to54` with whatever migration you require.

Sometimes a single error may mask several other issues.

!! TODO add references to migration projects like the phpcs fixer !!
!! TODO add vagrant setup !!
!! TODO extend usage section !!
