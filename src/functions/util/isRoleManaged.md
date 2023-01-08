---
title: $isRoleManaged 
description: $isRoleManaged will check if a certain role is managed by Discord.
id: isRoleManaged
---

`$isRoleManaged` will check if a certain role is managed by Discord.

## Usage

```php
$isRoleManaged[roleID;guildID?]
```

## Parameters 


| Field    | Type    | Description                                                             | Required |
| -------- | ------- | ----------------------------------------------------------------------- | -------- |
| roleID   | integer | role ID of the role you want to check if it's managed by Discord or not | yes      |
| guildID? | integer | guild ID of where the role exists                                       | no       |

### Please note that your bot has to be in the same server as the role or else this function will not work.

## Example

This will check if a role called `Server Booster` is managed by Discord and return either `true` or `false`:

```javascript
bot.command({
  name: 'isRoleManaged',
  code: `
  $isRoleManaged[$findRole[Server Booster];$guildID]
  `
});
```
