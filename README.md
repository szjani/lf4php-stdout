lf4php-stdout
==============

This is a Stdout binding for lf4php.

Using lf4php-stdout
--------------------

### Configuration

```php
<?php
LoggerFactory::setILoggerFactory(new StdoutLoggerFactory());
```

### Logging

```php
<?php
$logger = LoggerFactory::getLogger(null);
$logger->info('Message');
$logger->debug('Hello {{name}}!', array('name' => 'John'));
$logger->error(new \Exception());
```
