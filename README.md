# Circular Array

[![Build Status](https://goo.gl/7P7C7S)](https://travis-ci.org/PHPSnippets/CircularArray)
[![Minimum PHP Version](https://goo.gl/D13jNg)](https://php.net/)
[![Release](https://goo.gl/SpnYcX)](https://packagist.org/packages/php-snippets/circular-array)
[![Coverage Status](https://goo.gl/25u9F4)](https://scrutinizer-ci.com/g/PHPSnippets/CircularArray/code-structure)
[![Quality Score](https://goo.gl/RXk1Jy)](https://scrutinizer-ci.com/g/PHPSnippets/CircularArray)
[![Software License](https://goo.gl/QHtnq5)](LICENSE.md)


| ![](https://goo.gl/HGcdfB) |
|:---:|
| <sub>Image: [Cburnett](https://goo.gl/fCsXZT)</sub> |

From [Wikipedia](https://en.wikipedia.org/wiki/Circular_buffer):

>A [circular buffer](http://www.mathcs.emory.edu/~cheung/Courses/171/Syllabus/8-List/array-queue2.html), 
>circular queue, cyclic buffer or ring buffer is a data structure that uses a single, 
>[fixed-size buffer](http://php.net/manual/pt_BR/class.splfixedarray.php) as if it 
>were connected end-to-end.
>This structure lends itself easily to buffering data streams.

## Install

Via Composer

``` bash
$ composer require php-snippets/circular-array
```

## Usage

You can create an array where an interaction occurs indefinitely:

```php
use PHPSnippets\DataStructures\CircularArray;

$circular = Circular::fromArray(array(1, 2, 3, 4));

// this foreach never ends, after 4 back to 1.
foreach($circular as $value){
    echo $value;
}
```

## Requirements

The following versions of PHP are supported by this version.

* PHP >= 5.3

## Testing

```bash
$ vendor/bin/phpunit
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CONDUCT](CONDUCT.md) for details.

## Credits

- [Webysther Nunes](https://github.com/Webysther)
- [All Contributors](https://github.com/PHPSnippets/CircularArray/contributors)

## License

MIT. Please see [License File](LICENSE.md) for more information.
