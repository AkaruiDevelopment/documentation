---
title: $userBannerColor 
description: $userBannerColor will return the profile banner color.
id: userBannerColor
---

`$userBannerColor` will return the profile banner color.

## Usage

```php
$userBannerColor[userID?]
```

## Parameters 


| Field    | Type    | Description                                            | Required |
| -------- | ------- | ------------------------------------------------------ | :------: |
| userID?  | integer | the ID of the user                                     |    no    |


## Example

This will return your profile banner color:

```javascript
bot.command({
  name: 'userBanner',
  code: `
  $userBannerColor[$authorID]
  `
});
```
