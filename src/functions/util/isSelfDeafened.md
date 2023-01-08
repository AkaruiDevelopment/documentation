---
title: $isSelfDeafened 
description: $isSelfDeafened is similar but not to confuse with `$isDeafen`, this will check if the user deafened themselves.
id: isSelfDeafened
---

`$isSelfDeafened` is similar but not to confuse with `$isDeafen`, this will check if the user deafened themselves.

## Usage

```php
$isSelfDeafened[userid?;guildid?]
```

## Parameters 


| Field    | Type    | Description                                                   | Required |
| -------- | ------- | ------------------------------------------------------------- | -------- |
| userid?  | integer | the user id of the user you want to check if they're deafened | no       |
| guildid? | integer | the guild id of the guild where they're deafened in           | no       |


## Example

This will return either `true` or `false` depending on if you're deafened or not:

```javascript
bot.command({
  name: 'isSelfDeafened',
  code: `
  $isSelfDeafened
  `
});
```
