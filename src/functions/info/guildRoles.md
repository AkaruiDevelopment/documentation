---
title: $guildRoles 
description: $guildRoles will return all roles of a specific guild.
id: guildRoles
---

`$guildRoles` will return all roles of a specific guild.

## Usage

```php
$guildRoles[guildID?;option?;sep?]
```

## Parameters 


| Field    | Type    | Description                                        | Required  |
|----------|---------|----------------------------------------------------| :-------: |
| guildID? | integer | the ID of the guild                                | no       |
| option?  | string  | the option on how to return the roles <br> 1. **name** (default) <br> 2. **id** <br> 3. **mention**        | no       |
| sep?     | string  | seperator to seperate multiple arguments                    | no       |


## Example

This will return all roles of your guild:

```javascript
bot.command({
  name: 'guildRoles',
  code: `
  $description[$guildRoles[$guildID;name;, ]]
  `
});
```
