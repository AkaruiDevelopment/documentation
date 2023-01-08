---
title: $sub 
description: $sub will substract two given numbers.
id: sub
---

`$sub` will substract two given numbers.

## Usage

```php
$sub[num1;num2]
```

## Parameters 


| Field | Type   | Description | Required |
| ----- | ------ | ----------- | -------- |
| num1  | number |             | yes      |
| num2  | number |             | yes      |

## Example

This will return `65` as `70-5` equals `65`: 

```javascript
bot.command({
  name: 'sub',
  code: `
  $sub[70-5]
  `
});
```