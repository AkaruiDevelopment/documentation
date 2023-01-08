---
title: $findSpecialChars 
description: $findSpecialChars will return all special characters of the given argument.
id: findSpecialChars
---

`$findSpecialChars` will return all special characters of the given argument.

## Usage

```php
$findSpecialChars[text]
```

## Parameters 


| Field | Type   | Description                                    | Required |
| ----- | ------ | ---------------------------------------------- | -------- |
| text  | string | text where you want to find special characters | yes      |


## Example

This will return `######`:

```javascript
bot.command({
  name: 'findSpecialChars',
  code: `
  $findSpecialChars[Aoi.js is ###### great]
  `
});
```
