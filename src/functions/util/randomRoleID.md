---
title: $randomRoleID 
description: $randomRoleID will return a random role ID of a given guild.
id: randomRoleID
---

`$randomRoleID` will return a random role ID of a given guild.

## Usage

```php
$randomRoleID[guildID?]
```

## Parameters 


| Field    | Type    | Description                                  | Required |
| -------- | ------- | -------------------------------------------- | -------- |
| guildID? | integer | where it will return the random role ID from | yes      |


## Example

This will return a random role ID of your guild:

```javascript
bot.command({
  name: 'randomRoleID',
  code: `
  $randomRoleID[$guildID]
  `
});
```
