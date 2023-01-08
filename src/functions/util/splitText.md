---
title: $splitText 
description: $splitText will return a value of $textSplit depending on the given index.
id: splitText
---

`$splitText` will return a value of $textSplit depending on the given index.

## Usage

```php
$splitText[index]
```

## Parameters 


| Field | Type    | Description                  | Required |
| ----- | ------- | ---------------------------- | -------- |
| index | integer | index of $textSplit argument | yes      |


## Example

This will return `aoi.js` as it's the second argument of `$textSplit`: 

```javascript
bot.command({
  name: 'splitText',
  code: `
  $splitText[2]
  $textSplit[aoi.db//aoi.js;//]
  `
});
```