---
title: $isRoleEditable 
description: $isRoleEditable will check if the role is editable.
id: isRoleEditable
---

`$isRoleEditable` will check if the role is editable.

## Usage

```php
$isRoleEditable[roleid;guildid?]
```

## Parameters 


| Field    | Type    | Description                               | Required |
| -------- | ------- | ----------------------------------------- | -------- |
| roleid   | integer | role id you want to check if its editable | yes      |
| guildid? | integer | the guild id of where the role exists     | no       |


## Example

This will check if a role called `Owner` is editable:

```javascript
bot.command({
  name: 'isRoleEditable',
  code: `
  $isRoleEditable[$findRole[Owner];$guildID]
  `
});
```
