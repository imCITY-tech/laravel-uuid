# Laravel UUID

The package provides UUID keys functionality for Eloquent models with one single trait.


## Usage

1. Add a trait to your model, and it will automatically set the UUID during model creation.

```
<?php

namespace App;

use Illuminate\Database\Eloquent\Model;
use Nevadskiy\Uuid\Uuid;

class Book extends Model
{
    use Uuid;
}
```

2. Update your migrations to specify UUID type for a primary key.

```
Schema::create('books', function (Blueprint $table) {
    $table->uuid('id');
});
```


## Installation

Install a package via composer.

```
composer require nevadskiy/laravel-uuid
```


## Requirements

- Laravel `6.0` or newer  
- PHP `7.2` or newer


## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.


## Contributing

Any contribution is **Welcome**.

Please see [CONTRIBUTING](CONTRIBUTING.md) for more information.


## Security

If you discover any security related issues, please [e-mail me](mailto:nevadskiy@gmail.com) instead of using the issue tracker.


## License

The MIT License (MIT). Please see [LICENSE](LICENSE.md) for more information.
