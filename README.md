
[![Source Code](http://img.shields.io/badge/source-coffeebreaks/route-blue.svg?style=flat-square)](https://github.com/Guilherme-fagundes/route)
[![PHP from Packagist](https://img.shields.io/packagist/php-v/coffeebreaks/route.svg?style=flat-square)](https://packagist.org/packages/coffeebreaks/route)
[![Latest Stable Version](https://poser.pugx.org/coffeebreaks/route/v)](//packagist.org/packages/coffeebreaks/route)
[![License](https://poser.pugx.org/coffeebreaks/route/license)](//packagist.org/packages/coffeebreaks/route)
[![Total Downloads](https://poser.pugx.org/coffeebreaks/route/downloads)](//packagist.org/packages/coffeebreaks/route)
[![Build](https://img.shields.io/scrutinizer/build/g/Guilherme-fagundes/route.svg?style=flat-square)](https://scrutinizer-ci.com/g/Guilherme-fagundes/route)
[![Quality Score](https://img.shields.io/scrutinizer/g/Guilherme-fagundes/route.svg?style=flat-square)](https://scrutinizer-ci.com/g/Guilherme-fagundes/route)

### ROUTE
<p>This class performs the route function</p>

#### Instalation
```bash
composer require coffeebreaks/route
```

### Config.php

```php
define('HOME', ""); // Base URI
define('THEME', ''); // Your theme
define('INCLUDE_PATH', 'themes'.DIRECTORY_SEPARATOR.THEME);
```


### .htaccess

```.htaccess
RewriteEngine On

Options All -indexes

RewriteCond %{SCRIPT_FILENAME} !-d
RewriteCond %{SCRIPT_FILENAME} !-f
RewriteRule ^(.*)$ index.php?url=$1 [L,QSA]
```