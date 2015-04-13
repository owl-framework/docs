Кэширование
===========

Owl provides a unified cache API (cache component) for most popular caching systems.

## Cache Usage

### Store an item

To store the item, you need to use a `save` method like:

```php
$id = 'you item id';
$data = 12345;
$lifetime = 3600; // 60s * 60 m = 1 hour in seconds

$cache->save($id, $data, $lifetime);
```

### Retrieving An Item

To retrieving the item, you need to use a `get` method like:

```php
$value = $cache->get($id);
```