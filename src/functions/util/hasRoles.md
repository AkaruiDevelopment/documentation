---
title: $hasRoles 
description: $hasRoles check if the provided user has the roles listed in the roles argument.
id: hasRoles
---

`$hasRoles` check if the provided user has the roles listed in the roles argument.

## Usage

```php
$hasRoles[guildID;userID;...roles]
```

## Parameters 


| Field   | Type    | Description                             | Required |
| ------- | ------- | --------------------------------------- | -------- |
| guildID | integer | guild ID where the roles are present in | yes      |
| userID  | integer | user ID of the user which has the roles | yes      |
| roles   | integer | the roles that will be checked for      | yes      |


## Example

This will return `true` when the user has the listed roles:

```javascript
bot.command({
  name: 'hasRoles',
  code: `
  $hasRoles[$guildID;$authorID;$findRole[Owner]]
  `
});
```
