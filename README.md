Slack API
=========

A super simple wrapper for Slack API

Requires > PHP 5.

Installation
------------

Download and include the php file.

Usage
-----

List users

  <?php
  $Slack = new Slack('xoxp-0123456789-0123456789-0123456789-1a1a11');
  print_r($Slack->call('users.list'));

Invite user to a channel

  <?php
  $Slack = new Slack('xoxp-0123456789-0123456789-0123456789-1a1a11');
  print_r($Slack->call('channels.invite', array(
    'channel' => 'C1234567890',
    'user' => 'U1234567890'
  )));