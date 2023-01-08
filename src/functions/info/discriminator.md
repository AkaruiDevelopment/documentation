---
title: $discriminator 
description: $discriminator will return a user's discriminator.
id: discriminator
---

`$discriminator` will return a user's discriminator.

## Usage

```php
$discriminator[userId?]
```

## Parameters 


| Field   | Type    | Description                                           | Required |
| ------- | ------- | ----------------------------------------------------- | -------- |
| userId? | integer | the user id of the user you want the discriminator of | no       |


## Example

This will return your Discord User Discriminator, for example `0000`:

```javascript
bot.command({
  name: 'discriminator',
  code: `
  $discriminator[$authorID] // your discriminator
  $discriminator[$clientID] // the bot's discriminator
  `
});
```