Кэширование
===========
#### [Code documentation](https://framework.lowl.io/code/current/namespace/Owl/Cache.html) :: [PHP Stubs](https://github.com/owl-framework/owl/tree/master/ide/Owl/cache) :: [Source code](https://github.com/owl-framework/owl/tree/master/owl/Cache)

Owl предоставляет стандартизированный API (компонент) для популярных систем используемых в кэшировании данных.

## When is it needed?

Although this component is very fast, implementing it in cases that are not needed could lead to a loss of performance rather than gain.
We recommend you check this cases before using a cache:

* You are making complex calculations that every time return the same result (changing infrequently)
* You are using a lot of backends for future information building (for next time get from cache system by 1 query)
* You are accessing database data constantly and these data rarely change

## Quick Start

Caching adapters can either be created from the provided `Owl\Cache\Service` factory, or by simply instantiating one of the `Owl\Cache\Driver\*` classes.

```php
$cache = new \Owl\Cache\Driver\Memcached();
```

### Store an item

To store the item, you need to use a `save($id, $data, $lifeTime = 3600)` method like:

```php
$id = 'you item id';
$data = 12345;
$lifetime = 3600; // 60s * 60 m = 1 hour in seconds

$cache->save($id, $data, $lifetime);
```

### Retrieving An Item

To retrieving the item, you need to use a `get($id)` method like:

```php
$value = $cache->get($id);
```
