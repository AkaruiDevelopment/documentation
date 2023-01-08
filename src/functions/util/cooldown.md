---
title: $cooldown 
description: $cooldown will set a cooldown for the author of the command after being used.
id: cooldown
---

`$cooldown` will set a user-based cooldown.

## Usage

```php
$cooldown[time;errorMessage?]
```
* You are able to retrieve the remaining cooldown in the `$cooldown` function by using **`%time%`**.

## Parameters 


| Field         | Type   | Description                                                | Required |
| ------------- | ------ | ---------------------------------------------------------- | -------- |
| time          | string | the duration of the cooldown                               | yes      |
| errorMessage? | string | error message when there's remaining time for the cooldown | no       |


## Example

This will set a cooldown for a command which applies to the user only and returns the remaining cooldown:

```javascript
bot.command({
  name: 'cooldown',
  code: `
  hello
  $cooldown[2m;Please wait %time% to execute this command again.]
  `
});
```
