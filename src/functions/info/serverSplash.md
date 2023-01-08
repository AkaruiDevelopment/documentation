---
title: $serverSplash 
description: $serverSplash will return a guild's invite background (if unlocked).
id: serverSplash
---

`$serverSplash` will return a guild's invite background (if unlocked).

## Usage

```php
$serverSplash[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the server's invite background (if unlocked):

```javascript
bot.command({
  name: 'serverSplash',
  code: `
  $serverSplash[$guildID]
  `
});
```
