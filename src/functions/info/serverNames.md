---
title: $serverNames 
description: $serverNames will return the guide names your bot is in.
id: serverNames
---

`$serverNames` will return the guide names your bot is in.

## Usage

```php
$serverNames[sep?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| sep?    | string  | seperator to seperate multiple arguments                             | no      |


## Example

This will return the names of the guilds your bot is in and seperate it by a comma:

```javascript
bot.command({
  name: 'serverNames',
  code: `
  $serverNames[, ]
  `
});
```
