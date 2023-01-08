---
title: $sum 
description: $sum will sum-up two given numbers.
id: sum
---

`$sum` will sum-up two given numbers.

## Usage

```php
$sum[num1;num2]
```

## Parameters 


| Field | Type   | Description | Required |
| ----- | ------ | ----------- | -------- |
| num1  | number |             | yes      |
| num2  | number |             | yes      |

## Example

This will return `75` as `70+5` equals `75`: 

```javascript
bot.command({
  name: 'sum',
  code: `
  $sum[70+5]
  `
});
```