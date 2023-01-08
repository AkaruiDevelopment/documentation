---
title: $serverBoostLevel 
description: $serverBoostLevel will return the guild's boost level.
id: serverBoostLevel
---

`$serverBoostLevel` will return the guild's boost level.

## Usage

```php
$serverBoostLevel[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the boost level of a specific guild:

```javascript
bot.command({
  name: 'serverBoostLevel',
  code: `
  $serverBoostLevel[$guildID]
  `
});
```
