---
title: $truncate 
description: $truncate will remove all values after a decimal point.
id: truncate
---

`$truncate` will remove all values after a decimal point.

## Usage

```php
$truncate[number]
```

## Parameters 


| Field  | Type   | Description       | Required |
| ------ | ------ | ----------------- | -------- |
| number | number | value to truncate | yes      |


## Example

This will return `775` and remove `.9723` from the given value:

```javascript
bot.command({
  name: 'truncate',
  code: `
  $truncate[775.9723]
  `
});
```