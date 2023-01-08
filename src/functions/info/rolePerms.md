---
title: $rolePerms 
description: $rolePerms will return all given permissions of a role.
id: rolePerms
---

`$rolePerms` will return all given permissions of a role.

## Usage

```php
$rolePerms[roleID;sep?;guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| roleID    | integer  | role ID                             | yes      |
| sep?    | integer  | seperator to seperate multiple arguments                             | no      |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the permissions for the `@everyone` role:

```javascript
bot.command({
  name: 'rolePerms',
  code: `
  $rolePerms[$guildID;, ;$guildID]
  `
});
```
