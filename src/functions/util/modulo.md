---
title: $modulo
description: $modulo operation / the remainder when dividing.
id: modulo
---

`$modulo` operation / the remainder when dividing.

## Usage

```php
$modulo[...numbers;...numbers]
```

## Parameters 


| Field   | Type   | Description    | Required |
| ------- | ------ | -------------- | -------- |
| numbers | number | math operation | yes      |


## Example

This will return `2` as it's the remainder of `5 % 3`:

```javascript
bot.command({
  name: 'modulo',
  code: `
  $modulo[5;3]
  `
});
```
