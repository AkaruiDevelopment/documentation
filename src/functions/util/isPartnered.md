---
title: $isPartnered 
description: $isPartnered checks if the given guild is partnered with Discord.
id: isPartnered
---

`$isPartnered` checks if the given guild is partnered with Discord.

## Usage

```php
$isPartnered[guildID?]
```

## Parameters 


| Field    | Type    | Description                                                           | Required |
| -------- | ------- | --------------------------------------------------------------------- | -------- |
| guildID? | integer | the guild ID of the guild you want to check its partnership status of | yes      |


## Example

This will check if your server is partnered and return either `true` or `false`:

```javascript
bot.command({
  name: 'isPartnered',
  code: `
  $isPartnered[$guildID]
  `
});
```
