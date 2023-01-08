---
title: $getUserBadges 
description: $getUserBadges will return the given users' badges.
id: getUserBadges
---

`$getUserBadges` will return the given users's badges.

## Usage

```php
$getUserBadges[userId?;sep?]
```

## Parameters 


| Field   | Type    | Description                                                          | Required |
| ------- | ------- | -------------------------------------------------------------------- | :------: |
| userId? | integer | the id of the user you want the badges of                            |    no    |
| sep?    | string  | seperator to split multiple badges from eachother <br> `,` (default) |    no    |


## Example

This will return your Discord Badges seperated by a comma:

```javascript
bot.command({
  name: 'getUserBadges',
  code: `
  $getUserBadges[$authorID;, ]
  `
});
```