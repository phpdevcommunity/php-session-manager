# PHP - $_SESSION MANAGER
### A simple PHP Session Manager
[![Latest Stable Version](https://poser.pugx.org/devcoder-xyz/php-session-manager/v)](//packagist.org/packages/devcoder-xyz/php-session-manager) [![Total Downloads](https://poser.pugx.org/devcoder-xyz/php-session-manager/downloads)](//packagist.org/packages/devcoder-xyz/php-session-manager) [![Latest Unstable Version](https://poser.pugx.org/devcoder-xyz/php-session-manager/v/unstable)](//packagist.org/packages/devcoder-xyz/php-session-manager) [![License](https://poser.pugx.org/devcoder-xyz/php-session-manager/license)](//packagist.org/packages/devcoder-xyz/php-session-manager)

*PHP version required 7.3*

**How to use ?**
```php
$session = new \DevCoder\SessionManager();
$session->set('token', 'hash');

var_dump($session->get('token'));
// hash
$session->remove('token');
var_dump($session->get('token'));
// NULL
```

```php
$session = new \DevCoder\SessionManager();
$session->set('date', new \DateTime());
var_dump($session->get('date'));
// class DateTime#2 (3) {
//  public $date =>
//  string(26) "2020-11-14 22:17:39.128909"
//  public $timezone_type =>
//  int(3)
//  public $timezone =>
//  string(13) "Europe/Berlin"
}

$session->clear();
var_dump($session->get('date'));
// NULL
```

Simple and easy!
