---
title: $globalCooldown 
description: $globalCooldown will set a global-based cooldown for a command.
id: globalCooldown
---

`$globalCooldown` will set a global-based cooldown for a command.

## Usage

```php
$globalCooldown[time;errorMessage?]
```
* You are able to retrieve the remaining cooldown in the `$globalCooldown` function by using **`%time%`**.

## Parameters 


| Field         | Type   | Description                                                     | Required |
| ------------- | ------ | --------------------------------------------------------------- | -------- |
| time          | string | the duration of the cooldown                                    | yes      |
| errorMessage? | string | error message given when there's remaining time of the cooldown | no       |


## Example

This will return `Hello` and stop anyone from executing the command again for another five minutes:

```javascript
bot.command({
  name: 'globalCooldown',
  code: `
  Hello
  $globalCooldown[5m;Please wait %time% to execute this command again.]
  `
});
```
