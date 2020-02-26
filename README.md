# Nova Scheduled Jobs

[![Latest Version on Packagist](https://img.shields.io/packagist/v/llaski/nova-scheduled-jobs.svg?style=flat-square)](https://packagist.org/packages/llaski/nova-scheduled-jobs)
[![Total Downloads](https://img.shields.io/packagist/dt/llaski/nova-scheduled-jobs.svg?style=flat-square)](https://packagist.org/packages/llaski/nova-scheduled-jobs)

## Includes both a tool and card to display your scheduled commands and jobs

![Nova Scheduled Jobs Tool Screenshot](https://raw.githubusercontent.com/llaski/screenshots/master/nova-scheduled-jobs-tool.png)

![Nova Scheduled Jobs Card Screenshot](https://raw.githubusercontent.com/llaski/screenshots/master/nova-scheduled-jobs-card.png)

## Installation

You can install the package in to a Laravel app that uses [Nova](https://nova.laravel.com) via composer:

```bash
composer require parfumix/nova-scheduled-jobs
```

To setup the tool, you must register the tool with Nova. This is typically done in the `tools` method of the `NovaServiceProvider`.

```php
// in app/Providers/NovaServiceProvider.php

// ...

public function tools()
{
    return [
        // ...
        new \Llaski\NovaScheduledJobs\NovaScheduledJobsTool,
    ];
}
```

To setup the card, you must register the card with Nova. This is typically done in the `cards` method of the `NovaServiceProvider`.

```php
// in app/Providers/NovaServiceProvider.php

// ...

public function cards()
{
    return [
        // ...
        new \Llaski\NovaScheduledJobs\NovaScheduledJobsCard,
    ];
}
```

### Testing

``` bash
phpunit
```

### Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

### Security

If you discover any security related issues, please email larry.laski@gmail.com instead of using the issue tracker.

## Credits

- [Larry Laski](https://github.com/llaski)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
