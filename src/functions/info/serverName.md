---
title: $serverName 
description: $serverName will return a guild's name.
id: serverName
---

`$serverName` will return a guild's name.

## Usage

```php
$serverName[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the name of your guild:

```javascript
bot.command({
  name: 'serverName',
  code: `
  $serverName[$guildID]
  `
});
```
