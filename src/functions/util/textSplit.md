---
title: $textSplit 
description: $textSplit
id: textSplit
---

`$textSplit` 

## Usage

```php
$textSplit[text;sep?]
```

## Parameters 


| Field | Type   | Description                      | Required |
| ----- | ------ | -------------------------------- | -------- |
| text  | string | query of arguments               | yes      |
| sep?  | string | seperator for the text arguments | no       |


## Example

This will return `hello, how are you`: 

```javascript
bot.command({
  name: 'textSplit',
  code: `
  $splitText[1] $splitText[3] $splitText[6] $splitText[7]
  $textSplit[hello,__blurr__how__ayaka__leref__are__you;__]
  `
});
```