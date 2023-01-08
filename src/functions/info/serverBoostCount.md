---
title: $serverBoostCount 
description: $serverBoostCount will return the guild's boost count.
id: serverBoostCount
---

`$serverBoostCount` will return the guild's boost count.

## Usage

```php
$serverBoostCount[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the amount of boosts a specific guild has:

```javascript
bot.command({
  name: 'serverBoostCount',
  code: `
  $serverBoostCount[$guildID]
  `
});
```
