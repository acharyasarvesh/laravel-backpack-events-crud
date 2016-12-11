# SeanDowney\BackpackEventsCrud

[![Latest Version on Packagist][ico-version]](link-packagist)
[![Software License][ico-license]](LICENSE.md)
[![Total Downloads][ico-downloads]][link-downloads]

An admin interface to easily add/edit/remove Events, using [Laravel Backpack](laravelbackpack.com).

## Install

1) In your terminal:

``` bash
$ composer require seandowney/backpackeventscrud
```

2) Add the service provider to your config/app.php file:
```php
SeanDowney\BackpackEventsCrud\EventsCRUDServiceProvider::class,
```

3) Publish the config file & run the migrations
```bash
$ php artisan vendor:publish --provider="SeanDowney\BackpackEventsCrud\EventsCRUDServiceProvider" #publish config, view  and migration files
$ php artisan migrate #create the events tabl
```

4) [Optional] Add a menu item for it in resources/views/vendor/backpack/base/inc/sidebar.blade.php or menu.blade.php:

```html
<li><a href="{{ url(config('backpack.base.route_prefix', 'admin').'/event') }}"><i class="fa fa-file-o"></i> <span>Events</span></a></li>
```

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.


## Testing

``` bash
// TODO
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email hello@tabacitu.ro instead of using the issue tracker.

## Credits

- Seán Downey - Lead Developer
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/seandowney/backpackeventscrud.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/seandowney/backpackeventscrud.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/seandowney/backpackeventscrud
[link-downloads]: https://packagist.org/packages/seandowney/backpackeventscrud
[link-contributors]: ../../contributors
