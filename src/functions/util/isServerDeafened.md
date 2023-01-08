---
title: $isServerDeafened 
description: $isServerDeafened is similar but not to confuse with `$isDeafen`, this will check if the user is server deafened.
id: isServerDeafened
---

`$isServerDeafened` is similar but not to confuse with `$isDeafen`, this will check if the user is server deafened.

## Usage

```php
$isServerDeafened[userid?;guildid?]
```

## Parameters 


| Field    | Type    | Description                                                          | Required |
| -------- | ------- | -------------------------------------------------------------------- | -------- |
| userid?  | integer | the user id of the user you want to check if they're server deafened | no       |
| guildid? | integer | the guild id of the guild where they're server deafened in           | no       |


## Example

This will return either `true` or `false` depending on if you're server deafened or not:

```javascript
bot.command({
  name: 'isServerDeafened',
  code: `
  $isServerDeafened
  `
});
```
