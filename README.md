php-migration-standards
=======================

Migration tests using PHP_CodeSniffer standards.

This composer _metapackage_ provides tests between any two of these PHP versions:
* PHP 4.4
* PHP 5.0
* PHP 5.1
* PHP 5.2
* PHP 5.3
* PHP 5.4
* PHP 5.5

Please note that the tests are under development and will not yet cover much of the changelog.
Status changes will be reflected in later revisions of this README.

As with other standards tests only inform you what might cause conflicts but do not try to fix them for you.

install
-------

Git clone this repository and composer install the standards.

Or _require_ `php-migrations/standards` using composer.

PHP 5.3.2 or newer is required.

usage
-----

From with the `php-migration-standards` directory run
```
./vendor/bin/phpcs --standard=PHP52to54 /path/to/your/code
```
And replace `PHP52to54` with whatever migration you require.

Please note that smaller steps are recommended.
They reduce the number of reported standards violations and are faster to run and fix especially for larger/ older projects.

As with other standards it might happen that you fix an error and a new one occurs for that file. Sometimes a single error may mask several other issues. 

!! TODO add references to migration projects like the phpcs fixer !!
!! TODO add vagrant setup !!
!! TODO add detailed status information (links) !!
!! TODO add detailed install and usage information !!
