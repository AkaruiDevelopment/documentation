---
title: $memberAvatar 
description: $memberAvatar will return the profile picture of a guild member.
id: memberAvatar
---

`$memberAvatar` will return the profile picture of a guild member.

## Usage

```php
$memberAvatar[guildID?;userID?;size?;dynamic?;format?]
```

## Parameters 


| Field    | Type    | Description                                            | Required |
| -------- | ------- | ------------------------------------------------------ | :------: |
| guildID? | integer | the ID of the guild                                    |    no    |
| userID?  | integer | the ID of the member                                   |    no    |
| size?    | integer | the size of the image                                  |    no    |
| dynamic? | string  | dynamic image <br> 1. **yes** (default) <br> 2. **no** |    no    |
| format?  | string  |                                                        |    no    |


## Example

This will return your profile picture:

```javascript
bot.command({
  name: 'memberAvatar',
  code: `
  $memberAvatar[$guildID;$authorID;2048;yes;webp]
  `
});
```
