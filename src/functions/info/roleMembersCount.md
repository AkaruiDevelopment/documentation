---
title: $roleMembersCount 
description: $roleMembersCount will return the amount of members who have a specific role.
id: roleMembersCount
---

`$roleMembersCount` will return the amount of members who have a specific role.

## Usage

```php
$roleMembersCount[roleID;guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| roleID    | integer  | role ID                                           | yes      |
| guildID?    | integer  | guild ID                                        | no      |


## Example

This will return the amount of users who have a specific role:

```javascript
bot.command({
  name: 'roleMembersCount',
  code: `
  $roleMembersCount[$guildID;$guildID] //you can replace the first $guildID with any role ID you like
  `
});
```
