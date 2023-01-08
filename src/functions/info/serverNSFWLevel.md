---
title: $serverNSFWLevel 
description: $serverNSFWLevel will return the guild's NSFW level.
id: serverNSFWLevel
---

`$serverNSFWLevel` will return the guild's NSFW level.

## Usage

```php
$serverNSFWLevel[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | yes      |


## Example

This will return the guild's NSFW level:

```javascript
bot.command({
  name: 'serverNSFWLevel',
  code: `
  $serverNSFWLevel[$guildID]
  `
});
```
