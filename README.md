Slack API
=========

A super simple wrapper for Slack API

Requires > PHP 5.

Installation
------------

Download and include the php file.

Usage
-----

> See more methods on the [Slack API documentation](https://api.slack.com/methods).

List users

```php
$Slack = new Slack('xoxp-0123456789-0123456789-0123456789-1a1a11');
print_r($Slack->call('users.list'));
```

Invite user to a channel

```php
$Slack = new Slack('xoxp-0123456789-0123456789-0123456789-1a1a11');
print_r($Slack->call('channels.invite', array(
  'channel' => 'C1234567890',
  'user' => 'U1234567890'
)));
```

Author
-------

- [Low Yong Zhen](mailto:yz@stargate.io)

License
-------

Copyright (c) 2014

Licensed under the [MIT License](http://yzlow.mit-license.org/).