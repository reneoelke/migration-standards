php-migration-standards
=======================

This composer package provides compatibility tests between any two of these PHP versions:
* PHP 5.2
* [PHP 5.3](https://github.com/php-migrations/PHP52to53)
* [PHP 5.4](https://github.com/php-migrations/PHP53to54)
* [PHP 5.5](https://github.com/php-migrations/PHP54to55)

Please refer to each standard for further detail.

As with most phpcs standards code will not be modified directly and any error may mask further issues.

install
-------

Either

```
git clone git@github.com:php-migrations/migration-standards.git
cd migrations-standards
composer install
```

Or add `php-migrations/standards` to the _require_/ _require-dev_ section of your `composer.json`.

usage
-----

Test compatibility between two versions like

```
./vendor/bin/compat --from=52 --with=54 /path/to/your/code
```

Additionally any [phpcs](http://pear.php.net/manual/en/package.php.php-codesniffer.usage.php) argument can be used - but `--standard`.

!! TODO add vagrant setup !!

!! TODO extend usage section !!

!! TODO add references to migration projects like the phpcs fixer !!

!! TODO add travis integration notice !!
