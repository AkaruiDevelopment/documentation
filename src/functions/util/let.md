---
title: $let 
description: $let is used for storing temporary variables.
id: let
---

`$let` will store temporary variables which can be retrieved by `$get`.

## Usage

```php
$let[varname;value]
```

## Parameters 


| Field   | Type   | Description                                      | Required |
| ------- | ------ | ------------------------------------------------ | -------- |
| varname | string | name of the temporary variable                   | yes      |
| value   | string | value of the temporary variable you want to save | yes      |

## Example

This will return `Ayaka` from `$get`:

```javascript
bot.command({
  name: 'let',
  code: `
$get[genius]
$let[genius;Ayaka]
`
});
```
