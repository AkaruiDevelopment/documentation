---
title: $tempCooldown 
description: $tempCooldown will create a temporary cooldown for a command.
id: tempCooldown
---

`$tempCooldown` will create a temporary cooldown for a command.

## Usage

```php
$tempCooldown[time;id;errorMessage?]
```
* You are able to retrieve the remaining cooldown in the `$tempCooldown` function by using **`%time%`**.

## Parameters 


| Field         | Type   | Description                                                | Required |
| ------------- | ------ | ---------------------------------------------------------- | -------- |
| time          | string | the duration of the cooldown                               | yes      |
| id            | string |                                                            | yes      |
| errorMessage? | string | error message when there's remaining time for the cooldown | no       |


## Example

This will set a temporary cooldown for a command which applies once only:

```javascript
bot.command({
  name: 'tempCooldown',
  code: `
  hello
  $tempCooldown[2m;customid;Please wait %time% to execute this command again.]
  `
});
```
