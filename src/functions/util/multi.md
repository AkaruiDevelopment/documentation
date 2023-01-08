---
title: $multi 
description: $multi operation / multiplication.
id: multi
---

`$multi` will multiplicate given numbers.

## Usage

```php
$multi[...numbers;...numbers]
```

## Parameters 


| Field   | Type   | Description                  | Required |
| ------- | ------ | ---------------------------- | -------- |
| numbers | number | numbers you want to multiply | yes      |

## Example

This will return `72` as `8*9` equals that:

```javascript
bot.command({
  name: 'multi',
  code: `
  $multi[8;9]
  `
});
```
