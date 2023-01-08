---
title: $numberSeperator 
description: $numberSeperator will seperate numbers and make them readable.
id: numberSeperator
---

`$numberSeperator` will seperate numbers and make them readable.

## Usage

```php
$numberSeperator[num;sep?]
```

## Parameters 


| Field | Type   | Description                                                        | Required |
| ----- | ------ | ------------------------------------------------------------------ | -------- |
| num   | number | number you want to seperate                                        | yes      |
| sep?  | string | seperator which will be used to seperate the numbers, default: `,` | no       |


## Example

This will return `1,000,000`:

```javascript
bot.command({
  name: 'numberSeperator',
  code: `
  $numberSeperator[1000000;,]
  `
});
```
