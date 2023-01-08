---
title: $random 
description: $random will generate a random number between your chosen span.
id: random
---

`$random` will generate a random number between your chosen span.

## Usage

```php
$random[num1;num2;allow?;random?]
```

## Parameters 


| Field                         | Type   | Description                           | Required |
| ----------------------------- | ------ | ------------------------------------- | -------- |
| num1                          | number | start of the span                     | yes      |
| num2                          | number | end of the span                       | yes      |
| allow?                        | string | allows returning of decimal numbers   | no       |
| [random?](#advanced-examples) | string | if the returned number will be random | no       |


## Examples

This will return a random number between `20` and `250`:

```javascript
bot.command({
  name: 'random',
  code: `
  $random[20;250]
  `
});
```

### Advanced Examples

This will return a random decimal number between `25` and `50`:

```javascript
bot.command({
  name: 'random',
  code: `
  $random[25;50;yes]  
  `
});
```

This will return a random integer between `20` and `250` and the second `$random` will be random as well:

```javascript
bot.command({
  name: 'random',
  code: `
  $random[45;65;no;yes]
  $random[45;65;no;yes]
  `
});
```
