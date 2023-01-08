---
title: $lowestRole 
description: $lowestRole will return the lowest role of a specific user.
id: lowestRole
---

`$lowestRole` will return the lowest role of a specific user.

## Usage

```php
$lowestRole[userID?;guildID?]
```

## Parameters 


| Field    | Type    | Description                                     | Required |
| -------- | ------- | ----------------------------------------------- | :------: |
| userID?  | integer | user if of the user you want the lowest role of |    no    |
| guildID? | integer | the ID of the guild                             |    no    |


## Example

This will return the ID of your lowest role:

```javascript
bot.command({
  name: 'lowestRole',
  code: `
  $lowestRole[$authorID;$guildID]
  `
});
```
