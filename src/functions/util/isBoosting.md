---
title: $isBoosting 
description: $isBoosting will check if the given user is boosting the given guild.
id: isBoosting
---

`$isBoosting` will check if the given user is boosting the given guild.

## Usage

```php
$isBoosting[userID?;guildID?]
```

## Parameters 


| Field    | Type    | Description                                   | Required |
| -------- | ------- | --------------------------------------------- | -------- |
| userID?  | integer | user id to check if they're boosting          | no       |
| guildID? | integer | the guild id of where they boosted the server | no       |

### Please note that your bot has to be present in the server where you're going to check for an users boosting status.

## Example

This will return `false` or `true` depending on if you boosted this server:

```javascript
bot.command({
  name: 'isBoosting',
  code: `
  $isBoosting[$authorID;$guildID]
  `
});
```
