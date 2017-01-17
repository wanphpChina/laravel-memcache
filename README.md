## Laravel 5.3 Memcache Driver

If you're developing on Windows and you're having trouble setting up Memcached with Laravel.

Developed for using a taggable cache store and testing it locally on a Windows OS.

========

### Installation


Add the package to your composer.json and run composer update.

Update: added Laravel 5 support, not BC
```php
"wawa/memcache": "~2.0"
```


Add the memcache service provider in app/config/app.php:

```php
'Wawa\Memcache\MemcacheServiceProvider',
```

You may now update your config/cache.php config file to use memcache
```php
	'default' => 'memcache',
```

You may now update your config/session.php config file to use memcache

```php
	'driver' => 'memcache',
```
