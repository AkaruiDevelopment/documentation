---
title: $serverBanner 
description: $serverBanner will return the server banner of a given guild.
id: serverBanner
---

`$serverBanner` will return the server banner of a given guild.

## Usage

```php
$serverBanner[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return your server banner (if unlocked and using):

```javascript
bot.command({
  name: 'serverBanner',
  code: `
  $serverBanner[$guildID]
  `
});
```
