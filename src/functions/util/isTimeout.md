---
title: $isTimeout 
description: $isTimeout will check if the user is timeouted with Discord's built-in timeout feature.
id: isTimeout
---

`$isTimeout` will check if the user is timeouted with Discord's built-in timeout feature.

## Usage

```php
$isTimeout[guildid?;userid?]
```

## Parameters 


| Field    | Type    | Description                                | Required |
| -------- | ------- | ------------------------------------------ | -------- |
| guildid? | integer | the guild id of where they're timeouted in | no       |
| userid?  | integer | the user id of the user that's timeouted   | no       |


## Example

This will check if you're timeouted and either return `true` or `false`:

```javascript
bot.command({
  name: 'isTimeout',
  code: `
  $isTimeout[$guildID;$authorID]
  `
});
```
