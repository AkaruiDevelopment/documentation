---
title: $expandNumber 
description: $expandNumber will expand the given number.
id: expandNumber
---

`$expandNumber` will expand the given number.

## Usage

```php
$expandNumber[abbrNumber]
```

## Parameters 


| Field      | Type   | Description               | Required |
| ---------- | ------ | ------------------------- | -------- |
| abbrNumber | string | number you want to expand | yes      |


## Example

This will return `1300000`:

```javascript
bot.command({
  name: 'expandNumber',
  code: `
  $expandNumber[1.3m]`
});
```
