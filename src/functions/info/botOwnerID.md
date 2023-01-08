---
title: $botOwnerID 
description: $botOwnerID will return the user IDs of the bot owner (or of multiple people if you have a team).
id: botOwnerID
---

`$botOwnerID` will return the user IDs of the bot owner (or of multiple people if you have a team).

## Usage

```php
$botOwnerID[seperator?]
```

## Parameters 


| Field      | Type    | Description                                 | Required |
| ---------- | ------- | ------------------------------------------- | -------- |
| seperator? | integer | seperator to split user ids (default: `, `) | no       |


## Example

This will return your user ID:

```javascript
bot.command({
  name: 'botOwnerID',
  code: `
  $botOwnerID
  `
});
```