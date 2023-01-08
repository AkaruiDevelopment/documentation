---
title: $ordinal 
description: $ordinal adds st, nd, rd, th to a number such as 1st, 2nd, 3rd, 4th.
id: ordinal
---

`$ordinal` adds `st`, `nd`, `rd`, `th` to a number such as `1st`, `2nd`, `3rd`, `4th`.

## Usage

```php
$ordinal[number]
```

## Parameters 


| Field  | Type   | Description                                        | Required |
| ------ | ------ | -------------------------------------------------- | -------- |
| number | number | number which will add `st`, `nd`, `rd`, `th` to it | yes      |

## Example

```javascript
bot.command({
  name: 'ordinal',
  code: `
  $ordinal[12] // Returns 12nd 
  $ordinal[50] // Returns 50th
  $ordinal[11] // Returns 11st
  $ordinal[88] // Returns 88th
  `
});
```
