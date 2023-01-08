---
title: $serverAvailable 
description: $serverAvailable will return if the given guild is available on Discord.
id: serverAvailable
---

`$serverAvailable` will return if the given guild is available on Discord.

## Usage

```php
$serverAvailable[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?  | integer | guild ID                                           | no       |


## Example

This will return `true` or `false` depending on if the guild is available:

```javascript
bot.command({
  name: 'serverAvailable',
  code: `
  $serverAvailable[$guildID]
  `
});
```
