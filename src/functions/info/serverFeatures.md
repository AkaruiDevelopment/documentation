---
title: $serverFeatures 
description: $serverFeatures will return unlocked server features.
id: serverFeatures
---

`$serverFeatures` will return unlocked server features.

## Usage

```php
$serverFeatures[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the unlocked server features of a guild:

```javascript
bot.command({
  name: 'serverFeatures',
  code: `
  $serverFeatures[$guildID;yes]
  `
});
```
