---
title: $serverEmojis 
description: $serverEmojis will return the emojis of a specific guild.
id: serverEmojis
---

`$serverEmojis` will return the emojis of a specific guild.

## Usage

```php
$serverEmojis[sep?;guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| sep?     | string  | the seperator to seperate the returned emojis           | no       |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the emojis of your guild:

```javascript
bot.command({
  name: 'serverEmojis',
  code: `
  $serverEmojis[, ;$guildID]
  `
});
```
