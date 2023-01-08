---
title: $roleId 
description: $roleId will return the ID of a role.
id: roleId
---

`$roleId` will return the ID of a role.

## Usage

```php
$roleId[roleResolver;guildID?]
```

## Parameters 


| Field        | Type   | Description                                   | Required |
| ------------ | ------ | --------------------------------------------- | -------- |
| roleResolver | string | name of the role                              | yes      |
| guildID?     | string | id of the guild where the role was created in | no       |


## Example

This will return the role ID of a role called `Owner` (this example won't work if you dont have that role):

```javascript
bot.command({
  name: 'roleId',
  code: `
  $roleId[Owner;$guildID]
  `
});
```