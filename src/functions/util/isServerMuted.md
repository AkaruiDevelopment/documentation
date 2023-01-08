---
title: $isServerMuted 
description: $isServerMuted is similar but not to confuse with `$isMuted`, this will check if the user is server muted.
id: isServerMuted
---

`$isServerMuted` is similar but not to confuse with `$isMuted`, this will check if the user is server muted.

## Usage

```php
$isServerMuted[userid?;guildid?]
```

## Parameters 


| Field    | Type    | Description                                                       | Required |
| -------- | ------- | ----------------------------------------------------------------- | -------- |
| userid?  | integer | the user id of the user you want to check if they're server muted | no       |
| guildid? | integer | the guild id of the guild where they're server muted in           | no       |


## Example

This will return either `true` or `false` depending on if you're server muted or not:

```javascript
bot.command({
  name: 'isServerMuted',
  code: `
  $isServerMuted
  `
});
```
