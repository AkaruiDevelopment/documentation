---
title: $roundTenth
description: $roundTenth will round to the next tenth.
id: roundTenth
---

`$roundTenth` will round to the next tenth.

## Usage

```php
$roundTenth[number;decimalPosition?]
```

## Parameters 


| Field            | Type    | Description                           | Required |
| ---------------- | ------- | ------------------------------------- | -------- |
| number           | number  | number to round                       | yes      |
| decimalPosition? | integer | how many numbers after the comma come | no       |


## Example

This will return `503.70` as it's the nearest number to `503.6972`:

```javascript
bot.command({
  name: 'roundTenth',
  code: `
  $roundTenth[503.6972]
  `
});
```