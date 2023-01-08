---
title: $serverCooldown 
description: $serverCooldown will set a cooldown for the guild after being used.
id: serverCooldown
---

`$serverCooldown` will set a guild-based cooldown.

## Usage

```php
$serverCooldown[time;errorMessage?]
```
* You are able to retrieve the remaining cooldown in the `$serverCooldown` function by using **`%time%`**.

## Parameters 


| Field         | Type   | Description                                                | Required |
| ------------- | ------ | ---------------------------------------------------------- | -------- |
| time          | number | the duration of the cooldown                               | yes      |
| errorMessage? | string | error message when there's remaining time for the cooldown | no       |


## Example

This will set a cooldown for a command which applies to the guild only and returns the remaining cooldown:

```javascript
bot.command({
  name: 'serverCooldown',
  code: `
  hello
  $serverCooldown[2m;Please wait %time% to execute this command again.]
  `
});
```
