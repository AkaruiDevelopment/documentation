---
title: $getRoleColor 
description: $getRoleColor will return the given role's color.
id: getRoleColor
---

`$getRoleColor` will return the given role's color.

## Usage

```php
$getRoleColor[roleId;guildId?]
```

## Parameters 


| Field    | Type    | Description                                   | Required |
| -------- | ------- | --------------------------------------------- | :------: |
| roleId   | integer | the role Id of the role you want the color of |   yes    |
| guildId? | integer | the guild Id of where the role was created in |    no    |


## Example

This will return the role ID of your highest role:

```javascript
bot.command({
  name: 'getRoleColor',
  code: `
  $getRoleColor[$highestRole]
  `
});
```