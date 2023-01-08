---
title: $isDeafen 
description: $isDeafen will check if a certain user is deafened or not.
id: isDeafen
---

`$isDeafen` will check if a certain user is deafened or not.

## Usage

```php
$isDeafen[userID?;guildID?]
```

## Parameters 


| Field    | Type    | Description                                              | Required |
| -------- | ------- | -------------------------------------------------------- | -------- |
| userID?  | integer | user ID you want to check if they're deafened            | no       |
| guildID? | integer | the guild ID where you want to check if they're deafened | no       |


## Example

This will return `false` or `true` depending on if you're currently deafened or not:

```javascript
bot.command({
  name: 'isDeafen',
  code: `
  $isDeafen[$authorID;$guildID]
  `
});
```
