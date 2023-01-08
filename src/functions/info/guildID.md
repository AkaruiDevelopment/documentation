---
title: $guildID 
description: $guildID will return the guild ID of a given guild.
id: guildID
---

`$guildID` will return the guild ID of a given guild.

## Usage

```php
$guildID[name?]
```

## Parameters 


| Field     | Type    | Description                                        | Required   |
|-----------|---------|----------------------------------------------------| :--------: |
| name?     | string  | guild name you want the guild ID of                | no         |


## Example

This will return your guild ID:

```javascript
bot.command({
  name: 'guildID',
  code: `
  $guildID
  `
});
```
