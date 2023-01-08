---
title: $serverIcon 
description: $serverIcon will return the guild's icon.
id: serverIcon
---

`$serverIcon` will return the guild's icon.

## Usage

```php
$serverIcon[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | yes      |


## Example

This will return the icon of the guild:

```javascript
bot.command({
  name: 'serverIcon',
  code: `
  $serverIcon[$guildID]
  `
});
```
