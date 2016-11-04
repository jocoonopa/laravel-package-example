# Laravel Package Example

And example of a Laravel package.

- Load controllers
- Load routes
- Load views
- Load migrations
- Push middleware
- Bind Facade
- Publish configurations, resources, assets
- Use another package

### Installation

Add the package name to your composer.json:

```javascript
{
    "require": {
    	...,
        "yassine-khachlek/laravel-package-example": "dev-master"
    }
}
```

Then update using composer:

```
composer update
```

And add the service provider in config/app.php:

```php
Yk\LaravelPackageExample\LaravelPackageExampleProvider::class,
```

Then register Facade class aliase:

```php
'FacadeExample' => Yk\LaravelPackageExample\Facades\FacadeExample::class,
```

Publish assets:

```
php artisan vendor:publish
```

## License

### GPLv2

Copyright (c) 2016 Yassine Khachlek <yassine.khachlek@gmail.com>

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.