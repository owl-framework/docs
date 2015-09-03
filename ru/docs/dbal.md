DBAL
====
#### [Code documentation](https://framework.lowl.io/code/current/namespace/Owl/DBAL.html) :: [PHP Stubs](https://github.com/owl-framework/owl/tree/master/ide/Owl/dbal) :: [Source code](https://github.com/owl-framework/owl/tree/master/owl/DBAL)

Owl provides a unified cache API (cache component) for most popular caching systems.

## Why is it needed?


## Quick Start

First you need to setup a `Driver`:

```php
$driver = new \Owl\DBAl\Driver\Mysql(
    'mysql:host=127.0.0.1;dbname=phalcon-module-skeleton;port=49153',
    'root', //username
    'root', //password
    array(
        PDO::ATTR_PERSISTENT => true, // Example, PERSISTENT connection
        PDO::MYSQL_ATTR_INIT_COMMAND => 'SET NAMES "UTF8"' // Is needed to use utf8 in connection
    )
);
```

Next, you need to setup a connection using prepared driver:

```php
$connection = new \Owl\DBAL\Connection(['driver' => $driver], $eventManager);
$di->set('connection', $connection);```
```
