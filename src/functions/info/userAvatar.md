---
title: $userAvatar 
description: $userAvatar will return the profile picture of a specific user.
id: userAvatar
---

`$userAvatar` will return the profile picture of a specific user.

## Usage

```php
$userAvatar[userID?;size?;dynamic?;format?]
```

## Parameters 


| Field    | Type    | Description                                            | Required |
| -------- | ------- | ------------------------------------------------------ | :------: |
| userID?  | integer | the ID of the user                                     |    no    |
| size?    | integer | the size of the image                                  |    no    |
| dynamic? | string  | dynamic image <br> 1. **yes** (default) <br> 2. **no** |    no    |
| format?  | string  |                                                        |    no    |


## Example

This will return your profile picture:

```javascript
bot.command({
  name: 'userAvatar',
  code: `
  $userAvatar[$authorID;2048;yes;webp]
  `
});
```
