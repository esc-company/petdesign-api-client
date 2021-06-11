# Unofficial Petdesign API PhpClient

[![StyleCI](https://github.styleci.io/repos/267242299/shield?branch=master)](https://github.styleci.io/repos/267242299)

## About

This HttpClient used for connecting PETDESIGN API System.

It must required **KEY**.

## Install

```
composer require esc-company/petdesign-api-client
```

## Usage

## Lookup Petdesign Goods

You can use two method for fetch goods information.

They are `find()` and `get()`. `find` for **one** good information and `get` for goods information **list**.

```php
<?php

$good = (new Good({api_key}))->find(30);
$goods = (new Good({api_key}))->show(false)->get();
$goods = (new Good({api_key}))->page(1)->get();
$goods = (new Good({api_key}))->from('2019-09-01')->get();
```

We suggsest Fasade class for your convinient. As soon...

## Test

```bash
composer test
```

## License

The Phpunit Start Kit is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
