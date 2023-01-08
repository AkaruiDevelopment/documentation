---
title: $advanceCooldown 
description: $advanceCooldown will set a cooldown for a given ID.
id: advanceCooldown
---

`$advanceCooldown` will set a cooldown for a given ID.

## Usage

```php
$advanceCooldown[time;id;errorMessage?]
```

* You are able to retrieve the remaining cooldown in the `$cooldown` function by using **`%time%`**.

## Parameters 


| Field         | Type    | Description                                                   | Required |
| ------------- | ------- | ------------------------------------------------------------- | -------- |
| time          | string  | text to be seperated                                          | yes      |
| id            | integer | text to be seperated                                          | yes      |
| errorMessage? | string  | error message to be displayed when there's cooldown remaining | no       |


## Example

This will set a cooldown for the guild of where you execute the command in and return the remaining cooldown time:

```javascript
bot.command({
  name: 'advanceCooldown',
  code: `
  $advanceCooldown[2m;$guildID;]
  `
});
```