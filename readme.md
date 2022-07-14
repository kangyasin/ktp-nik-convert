# Laravel KTP NIK Convert

<p style="text-align: center;">
    <a href="https://github.com/Kangyasin/ktp-nik-convert/releases" title="Latest Stable Version">
        <img src="https://img.shields.io/github/release/Kangyasin/ktp-nik-convert.svg?style=flat-square" alt="Latest Stable Version">
    </a>
    <a href="https://packagist.org/packages/Kangyasin/ktp-nik-convert" title="Total Downloads">
        <img src="https://img.shields.io/packagist/dt/Kangyasin/ktp-nik-convert.svg?style=flat-square" alt="Total Downloads">
    </a>
    <a href="https://coveralls.io/github/Kangyasin/ktp-nik-convert?branch=main" title="Coverage Status">
        <img src="https://coveralls.io/repos/github/Kangyasin/ktp-nik-convert/badge.svg?branch=main" alt="Coverage Status">
    </a>
    <a href="/LICENSE.md" title="License: MIT">
        <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT">
    </a>
</p>

![Laravel API BNI by Kang Yasin](/ktp-nik-convert.jpeg)


Save time and take advantage of a set of dynamical, ready-to-use.
Found this package helpful ? Please consider supporting my work!

[![Donate](https://img.shields.io/badge/Buy_me_a-Ko--fi-ff5f5f.svg)](https://ko-fi.com/Kangyasin)
[![Donate](https://img.shields.io/badge/Donate_on-PayPal-green.svg)](https://paypal.me/Kangyasin)

Package laravel Check National Identity Number to Identity gender, birth of date, and region in Indonesia.

## Table of Contents

* [Installation](#installation)
* [Useage](#usage)

## Installation

You can install the package via composer:

```bash
composer require kangyasin/ktp-nik-convert
```

## Usage

```php
<?php

use Kangyasin\KTPNIKConvert\NikConvert;

$nik = '6408132511960005';
$nikConvert= new NikConvert();

return $nikConvert->convert($nik);
```

Response

```code
{
"nik": "6408132511960005",
"province": {
    "code": "64",
    "name": "Kalimantan Timur"
},
"city": {
    "code": "08",
    "name": "Kabupaten Kutai Timur"
},
"district": {
    "code": "13",
    "name": "Teluk Pandan"
},
"date_of_birth": "25-11-1996",
"gender": "Male"
}
```

## Documentation

Please refer to our extensive [Wiki documentation](https://github.com/Kangyasin/ktp-nik-convert/wiki) for more information.

