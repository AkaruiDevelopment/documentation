---
title: $round 
description: $round will round to the next whole number.
id: round
---

`$round` will round to the next whole number.

## Usage

```php
$round[number]
```

## Parameters 


| Field  | Type   | Description     | Required |
| ------ | ------ | --------------- | -------- |
| number | number | number to round | yes      |


## Example

This will return `555` as it's the next number to `555.78`:

```javascript
bot.command({
  name: 'round',
  code: `
  $round[555.78]
  `
});
```