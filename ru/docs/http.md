HTTP Layer
==========
#### [Code documentation](https://framework.lowl.io/code/current/) :: [PHP Stubs](https://github.com/owl-framework/owl/tree/master/ide/Owl/http/) :: [Source code](https://github.com/owl-framework/owl/tree/master/owl/Http)

## Overview

# The Request Class

The `Owl\Http\Request` object is responsible for providing a fluent API that allows a developer to interact with all the various parts of an HTTP request.

## Quick Start

Request objects can either be created from the provided `createFromGlobals`

```php
use Owl\Http\Request;

$request = Request::createFromGlobals();

var_dump($request->getScheme()); // string(4) "http"
```

## Available Methods

### getScheme();

Get request scheme (http/https)

```php
$request->getScheme();
```

###  getUri();

Get request URI

```php
$request->getScheme();
```

### getPath();

Get request path (URI without GET parameters)

```php
$request->getScheme();
```

### getParam(string! key, var defaultValue = null);

Get param from, similar $_GET

```php
$request->getParam('code');
```

### getPost(string! key, var defaultValue = null);

Get param from, similar $_GET

```php
$request->getPost('code');
```

### getServer(string! key, var defaultValue = null);

Get param from, similar $_GET

```php
$request->getServer('code');
```
