---
title: $isVerified 
description: $isVerified checks if the given guild is verified by Discord.
id: isVerified
---

`$isVerified` checks if the given guild is verified by Discord.

## Usage

```php
$isVerified[guildID?]
```

## Parameters 


| Field    | Type    | Description                                                            | Required |
| -------- | ------- | ---------------------------------------------------------------------- | -------- |
| guildID? | integer | the guild ID of the guild you want to check its verification status of | no       |


## Example

This will check if your server is verified and return either `true` or `false`:

```javascript
bot.command({
  name: 'isVerified',
  code: `
  $isVerified[$guildID]
  `
});
```
