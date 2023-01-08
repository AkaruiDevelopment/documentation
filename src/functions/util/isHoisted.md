---
title: $isHoisted 
description: $isHoisted will check if a specific role is hoisted.
id: isHoisted
---

`$isHoisted` will check if a specific role is hoisted.

## Usage

```php
$isHoisted[roleID;guildID?]
```

## Parameters 


| Field    | Type    | Description                                                                     | Required |
| -------- | ------- | ------------------------------------------------------------------------------- | -------- |
| roleID   | integer | role ID of the role you want to check if it's hoisted or not                    | yes      |
| guildID? | integer | the guild id of the guild where you want to check if the role is hoisted or not | no       |

### Please note that your bot has to be in the server in order for this function to work.

## Example

This will check if a role called `Owner` is hoisted in your server:

```javascript
bot.command({
  name: 'isHoisted',
  code: `
  $isHoisted[$findRole[Owner];$guildID]
  `
});
```
