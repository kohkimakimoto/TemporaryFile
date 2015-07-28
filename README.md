# TemporaryFile

[![Build Status](https://travis-ci.org/kohkimakimoto/TemporaryFile.svg)](https://travis-ci.org/kohkimakimoto/TemporaryFile)
[![Latest Stable Version](https://poser.pugx.org/kohkimakimoto/temporary-file/v/stable)](https://packagist.org/packages/kohkimakimoto/temporary-file) [![Total Downloads](https://poser.pugx.org/kohkimakimoto/temporary-file/downloads)](https://packagist.org/packages/kohkimakimoto/temporary-file) [![Latest Unstable Version](https://poser.pugx.org/kohkimakimoto/temporary-file/v/unstable)](https://packagist.org/packages/kohkimakimoto/temporary-file) [![License](https://poser.pugx.org/kohkimakimoto/temporary-file/license)](https://packagist.org/packages/kohkimakimoto/temporary-file)

A PHP helper class to manipulate a temporary file.

```php
use Kohkimakimoto\TemporaryFile\TemporaryFile;

$tmpfile = new TemporaryFile();

echo $tmpfile->path();  // ex) /private/var/folders/bt/xwh9qmcj00dctz53_rxclgtr0000gn/T/phpqWK5fj
$tmpfile->write("temporary data...");

echo $data = $tmpfile->read(); // temporary data...

// You don't need to close it. The temporary file will be closed automatically.
```

## Requirements

* PHP5.3 or later


## Installation

Create `composer.json` for installing via composer..

```
{
    "require": {
        "kohkimakimoto/temporary-file": "0.1.*"
    }
}
```

Run composer install command.

```
composer install
```

## Author

Kohki Makimoto <kohki.makimoto@gmail.com>

## License

MIT license.
