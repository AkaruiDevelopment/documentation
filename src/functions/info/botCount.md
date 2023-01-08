---
title: $botCount 
description: $botCount will return the amount of Bots in your guild.
id: banCount
---

`$botCount` will return the amount of Bots in your guild.

## Usage

```php
$botCount[guildID?]
```

## Parameters 


| Field    | Type    | Description                                                   | Required |
| -------- | ------- | ------------------------------------------------------------- | :------: |
| guildID? | integer | guild id of the guild you want to retrieve the amount of bots |    no    |


## Example

This will return the amount of bots in your guild:

```javascript
bot.command({
  name: 'botCount',
  code: `
  $botCount
  `
});
```