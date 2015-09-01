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
```

## Available Methods

getScheme(); - Get request scheme (http/https)
getUri(); - Get request URI
getPath(); - Get request path (URI without GET parameters)
getParam(string! key, var defaultValue = null); - Get param from $_GET
getPost(string! key, var defaultValue = null); - Get param from $_POST
getServer(string! key, var defaultValue = null); - Get param from $_SERVER
