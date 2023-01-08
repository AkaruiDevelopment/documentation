---
title: $randomUserID 
description: $randomUserID will return a random username.
id: randomUserID
---

`$randomUserID` will return a random username.

## Usage

```php
$randomUserID[global/guildID?]
```

## Parameters 


| Field           | Type   | Description                                                             | Required |
| --------------- | ------ | ----------------------------------------------------------------------- | -------- |
| global/guildID? | string | return a random user out of all guild or out of one specific guild only | no       |


## Example

This will return a random user id:

```javascript
bot.command({
  name: 'randomUserID',
  code: `
  $randomUserID[global]
  `
});
```
