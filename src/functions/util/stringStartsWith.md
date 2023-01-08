---
title: $stringStartsWith 
description: $stringStartsWith will check if the given argument starts with something specific.
id: stringStartsWith
---

`$stringStartsWith` will check if the given argument starts with something specific.

## Usage

```php
$stringStartsWith[text;check]
```

## Parameters 


| Field | Type   | Description                                                             | Required |
| ----- | ------ | ----------------------------------------------------------------------- | -------- |
| text  | string | the text that will be checked                                           | yes      |
| check | string | the argument that will check if the text starts with something specific | yes      |

## Example

This will return `true` as `aoi.js` starts with `aoi`: 

```javascript
bot.command({
  name: 'stringStartsWith',
  code: `
  $stringStartsWith[aoi.js;aoi]
  `
});
```