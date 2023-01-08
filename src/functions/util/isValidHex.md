---
title: $isValidHex 
description: $isValidHex will check if the given hex / decimal color is valid.
id: isValidHex
---

`$isValidHex` will check if the given hex / decimal color is valid.

## Usage

```php
$isValidHex[color/int]
```

## Parameters 


| Field     | Type           | Description                | Required |
| --------- | -------------- | -------------------------- | -------- |
| color/int | string/integer | hex / decimal color string | yes      |


## Example

This will return `true` as `#30dbd8` is an valid hex color:

```javascript
bot.command({
  name: 'isValidHex',
  code: `
  $isValidHex[#30dbd8]
  `
});
```

This will return `true` as well as `80` is an valid hexadecimal  color:


```javascript
bot.command({
  name: 'isValidHex',
  code: `
  $isValidHex[80]
  `
});
```
