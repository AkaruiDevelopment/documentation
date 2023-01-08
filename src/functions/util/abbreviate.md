---
title: $abbreviate
description: $abbreviate will allow you to abbreviate large numbers.
id: abbreviate
---

`$abbreviate` will allow you to abbreviate large numbers.

## Usage

```php
$abbreviate[num;dec?]
```

## Parameters 


| Field | Type    | Description                    | Required |
| ----- | ------- | ------------------------------ | -------- |
| num   | integer | number to abbreviate           | yes      |
| dec?  | integer | decimal between the abbreviate | no       |

## Example(s)

This returns: `20k`

```javascript
bot.command({
  name: 'abbreviate',
  code: `
  $abbreviate[20000]
  `
});
```

This returns: `20.0k`

```javascript
bot.command({
  name: 'abbreviate',
  code: `
  $abbreviate[20000;1]
  `
});
```
