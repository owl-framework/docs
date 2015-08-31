Cache
=====
#### [Code documentation](https://framework.lowl.io/code/current/namespace/Owl/Cache.html) :: [PHP Stubs](https://github.com/owl-framework/owl/tree/master/ide/Owl/cache) :: [Source code](https://github.com/owl-framework/owl/tree/master/owl/Cache)

Owl provides a unified cache API (cache component) for most popular caching systems.

## When is it needed?

Although this component is very fast, implementing it in cases that are not needed could lead to a loss of performance rather than gain.
We recommend you check this cases before using a cache:

* You are making complex calculations that every time return the same result (changing infrequently)
* You are using a lot of backends for future information building (for next time get from cache system by 1 query)
* You are accessing database data constantly and these data rarely change

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