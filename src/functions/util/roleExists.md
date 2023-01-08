---
title: $roleExists 
description: $roleExists will check if a certain role exists within a certain guild.
id: roleExists
---

`$roleExists` will check if a certain role exists within a certain guild.

## Usage

```php
$roleExists[roleId;guildId?]
```

## Parameters 


| Field    | Type    | Description                                 | Required |
| -------- | ------- | ------------------------------------------- | -------- |
| roleId   | integer | role ID you want to check if it exists      | yes      |
| guildId? | integer | guild ID of the guild where the role exists | no       |


## Example

This will return `false` as the role doesn't exist in your guide: 

```javascript
bot.command({
  name: 'roleExists',
  code: `
  $roleExists[900004369355931729;$guildID]
  `
});
```