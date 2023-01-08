---
title: $isMentionable 
description: $isMentionable check if a given role is mentionable.
id: isMentionable
---

`$isMentionable` check if a given role is mentionable.

## Usage

```php
$isMentionable[roleID;guildID?]
```

## Parameters 


| Field    | Type    | Description                                     | Required |
| -------- | ------- | ----------------------------------------------- | -------- |
| roleID   | integer | the role id to check if it's mentionable or not | yes      |
| guildID? | integer | guild id where the role is present in           | no       |

### Please note that your bot has to be in the same guild as the role for the function to work.

## Example

This will check if a role with the name `Owner` is mentionable and returns either `true` or `false`: 

```javascript
bot.command({
  name: 'isMentionable',
  code: `
  $isMentionable[$findRole[Owner];$guildID]
  `
});
```
