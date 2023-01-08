---
title: $isUserDmEnabled 
description: $isUserDmEnabled will check if the user's Direct Messages are either disabled or enabled.
id: isUserDmEnabled
---

`$isUserDmEnabled` will check if the user's Direct Messages are either disabled or enabled.

## Usage

```php
$isUserDmEnabled[userid]
```

## Parameters 


| Field  | Type    | Description                                                           | Required |
| ------ | ------- | --------------------------------------------------------------------- | -------- |
| userid | integer | user id of the user you want to check if their dms are enabled or not | yes      |


## Example

This will return either `true` or `false` depending on if your Direct Messages are enabled or disabled:

```javascript
bot.command({
  name: 'isUserDmEnabled',
  code: `
  $isUserDmEnabled[$authorID]
  `
});
```
