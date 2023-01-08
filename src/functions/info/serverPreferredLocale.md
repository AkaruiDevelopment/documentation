---
title: $serverPreferredLocale 
description: $serverPreferredLocale will return a guild's set locale.
id: serverPreferredLocale
---

`$serverPreferredLocale` will return a guild's set locale.

## Usage

```php
$serverPreferredLocale[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the guild's preferred locale:

```javascript
bot.command({
  name: 'serverPreferredLocale',
  code: `
  $serverPreferredLocale[$guildID]
  `
});
```
