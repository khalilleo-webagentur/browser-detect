## monolog

PHP library for Browser Detection in a simple way.

### Requirements

* PHP `^8.1`

### Installation

`composer require khalilleo-webagentur/browser-detect`

### Usage

```php

$userAgent = new UserAgent();

$userAgent->getBrowserName();
$userAgent->getBrowserLang();
$userAgent->getPlatform();
$userAgent->getReferer();
$userAgent->isMobile();
$userAgent->isBot();

```

### Example

```php
<?php

use Khalilleo\BrowserDetect\UserAgent;

require 'vendor/autoload.php';

$userAgent = new UserAgent();

var_dump($userAgent->getBrowserName()); // output: Mozilla Firefox
var_dump($userAgent->getPlatform()); // output: linux
var_dump($userAgent->getBrowserLang()); // output: en
var_dump($userAgent->getReferer()); // output: Unknown
var_dump($userAgent->isMobile()); // output: false
var_dump($userAgent->isBot()); // output: false

```

### Copyright

This project is licensed under the MIT License.
