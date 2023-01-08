---
title: $highestRole 
description: $highestRole will return the highest role of a specific user.
id: highestRole
---

`$highestRole` will return the highest role of a specific user.

## Usage

```php
$highestRole[userID?;guildID?;option?]
```

## Parameters 


| Field    | Type    | Description                                        | Required  |
|----------|---------|----------------------------------------------------| :-------: |
| userID?     | integer | user if of the user you want the highest role of           | no        |
| guildID? | integer | the ID of the guild                                | no        |
| option?  | string  | the option on how to return the role <br> 1. **name** <br> 2. **id** (default) <br> 3. **mention**        | no       |


## Example

This will return the name of your highest role:

```javascript
bot.command({
  name: 'highestRole',
  code: `
  $highestRole[$authorID;$guildID;name]
  `
});
```
