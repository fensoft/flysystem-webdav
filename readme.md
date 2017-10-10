# League\Flysystem\WebDAV [BETA]

[![Author](http://img.shields.io/badge/author-@frankdejonge-blue.svg?style=flat-square)](https://twitter.com/frankdejonge)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)

This is a Flysystem adapter for the WebDAV.

## Installation

```bash
composer require fensoft/flysystem-webdav
```

# Bootstrap

``` php
<?php
use Sabre\DAV\Client;
use League\Flysystem\Filesystem;
use League\Flysystem\WebDAV\WebDAVAdapter;

$client = new Client($settings);
$adapter = new WebDAVAdapter($client);
$flysystem = new Filesystem($adapter);
```
