---
title: $stringEndsWith 
description: $stringEndsWith will check if the given argument ends with something specific.
id: stringEndsWith
---

`$stringEndsWith` will check if the given argument ends with something specific.

## Usage

```php
$stringEndsWith[text;check]
```

## Parameters 


| Field | Type   | Description                                                           | Required |
| ----- | ------ | --------------------------------------------------------------------- | -------- |
| text  | string | the text that will be checked                                         | yes      |
| check | string | the argument that will check if the text ends with something specific | yes      |

## Example

This will return `true` as `aoi.js` ends with `js`: 

```javascript
bot.command({
  name: 'stringEndsWith',
  code: `
  $stringEndsWith[aoi.js;js]
  `
});
```