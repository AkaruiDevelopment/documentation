---
title: $roleIconURL 
description: $roleIconURL will retrieve the imagine URL of the role icon.
id: roleIconURL
---

`$roleIconURL` will retrieve the imagine URL of the role icon.

## Usage

```php
$roleIconURL[guildId?;roleId]
```

## Parameters


| Field    | Type    | Description                                 | Required |
| -------- | ------- | ------------------------------------------- | -------- |
| guildId? | integer | guild ID of the guild where the role exists | no       |
| roleId   | integer | role ID you want to check if it exists      | yes      |


## Example

This will return the image URL of the role icon: 

```javascript
bot.command({
  name: 'roleIconURL',
  code: `
  $roleIconURL[$guildID;900004369355931729]
  `
});
```