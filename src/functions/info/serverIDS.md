---
title: $serverIDS 
description: $serverIDS will return the ID of every guild your bot is in.
id: serverIDS
---

`$serverIDS` will return the ID of every guild your bot is in.

## Usage

```php
$serverIDS[sep?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| sep?      | string  | the seperator to seperate multiple argument        | no       |


## Example

This will return all guild IDs your bot is in:

```javascript
bot.command({
  name: 'serverIDS',
  code: `
  $serverIDS[, ]
  `
});
```
