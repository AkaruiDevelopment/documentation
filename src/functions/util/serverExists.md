---
title: $serverExists 
description: $serverExists will check if the given guild exists.
id: serverExists
---

`$serverExists` will check if the given guild exists.

## Usage

```php
$serverExists[guildId]
```

## Parameters 


| Field   | Type    | Description | Required |
| ------- | ------- | ----------- | -------- |
| guildId | integer | guild id    | yes      |


## Example

This will return `true` your guild exists:

```javascript
bot.command({
  name: 'serverExists',
  code: `
  $serverExists[$guildID]
  `
});
```