---
title: $isSelfMuted 
description: $isSelfMuted is similar but not to confuse with `$isMuted`, this will check if the user muted themselves.
id: isSelfDeafened
---

$isSelfMuted is similar but not to confuse with `$isMuted`, this will check if the user muted themselves.

## Usage

```php
$isSelfMuted[userid?;guildid?]
```

## Parameters 


| Field    | Type    | Description                                                | Required |
| -------- | ------- | ---------------------------------------------------------- | -------- |
| userid?  | integer | the user id of the user you want to check if they're muted | no       |
| guildid? | integer | the guild id of the guild where they're muted in           | no       |


## Example

This will return either `true` or `false` depending on if you're muted (voice channel) or not:

```javascript
bot.command({
  name: 'isSelfDeafened',
  code: `
  $isSelfDeafened
  `
});
```
