---
title: $roleName 
description: $roleName will return the name of a specific role.
id: roleName
---

`$roleName` will return the name of a specific role.

## Usage

```php
$roleName[roleID;guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| roleID    | integer  | role ID                             | yes      |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the role name of any role you may like, in this case, It would return `@everyone`:

```javascript
bot.command({
  name: 'roleName',
  code: `
  \`$roleName[$guildID]\`
  `
});
```
