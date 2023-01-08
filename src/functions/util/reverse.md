---
title: $reverse 
description: $reverse will reverse given text.
id: reverse
---

`$reverse` will reverse given text.

## Usage

```php
$reverse[text]
```

## Parameters 


| Field | Type   | Description              | Required |
| ----- | ------ | ------------------------ | -------- |
| text  | string | text you want to reverse | yes      |


## Example

This will the following text readable: 

```javascript
bot.command({
  name: 'reverse',
  code: `
  $reverse[!snoitalutargnoc neht ,siht daer ot elba er'uoy fi ,desrever si txet sihT]
  `
});
```