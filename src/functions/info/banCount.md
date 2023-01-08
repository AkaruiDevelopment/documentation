---
title: $banCount 
description: $banCount will return the amount of banned users of a specific guild.
id: banCount
---

`$banCount` will return the amount of banned users of a specific guild.

## Usage

```php
$banCount[guildID?]
```

## Parameters 


| Field    | Type    | Description                                                           | Required |
| -------- | ------- | --------------------------------------------------------------------- | -------- |
| guildID? | integer | guild id of the guild you want to retrieve the amount of banned users | no       |

#### Please note that your bot requires permissions to `VIEW_AUDIT_LOG`

## Example

This will return the amount of banned users in your guild:

```javascript
bot.command({
  name: 'banCount',
  code: `
  $banCount
  `
});
```