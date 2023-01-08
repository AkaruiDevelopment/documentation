---
title: $concatTextSplit 
description: $concatTextSplit will concatenates the text with the given separator.
id: concatTextSplit
---

`$concatTextSplit` will concatenates the text with the given separator.

## Usage

```php
$concatTextSplit[...text]
```

## Parameters 


| Field | Type   | Description          | Required |
| ----- | ------ | -------------------- | -------- |
| text  | string | text to be seperated | yes      |


## Example

This will add `Hello, Bye` to the already used `$textSplit` argument:

```javascript
bot.command({
  name: 'concatTextSplit',
  code: `
  $concatTextSplit[Hello;Bye]
  $textSplit[Goodmorning, Goodnight;, ]
  `
});
```
