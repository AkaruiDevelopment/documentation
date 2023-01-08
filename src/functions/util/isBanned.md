---
title: $isBanned 
description: $isBanned checks if a given user is banned in a specific guild.
id: isBanned
---

`$isBanned` checks if a given user is banned in a specific guild.

## Usage

```php
$isBanned[guildID;userID]
```

## Parameters 


| Field   | Type    | Description                                                  | Required |
| ------- | ------- | ------------------------------------------------------------ | -------- |
| guildID | integer | ID of the guild where to check if the user is banned or not  | yes      |
| userID  | integer | ID of the user that will be checked if they're banned or not | yes      |

### Please note that your bot has to be present in the guild and needs permissions to view audit logs for this function to function properly.

## Example

This will return `false` as you're not banned in this guild:

```javascript
bot.command({
  name: 'isBanned',
  code: `
  $isBanned[$authorID;$authorID]
  `
});
```
