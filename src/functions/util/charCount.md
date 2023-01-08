---
title: $charCount 
description: $charCount will count the given characters in a text and return the amount of characters.
id: charCount
---

`$charCount` will count the given characters in a text and return the amount of characters.

## Usage

```php
$charCount[text]
```

## Parameters 


| Field | Type   | Description                                           | Required |
| ----- | ------ | ----------------------------------------------------- | -------- |
| text  | string | the text that will be the character count returned of | yes      |


## Example

This will return `77` as there are 77 characters in this text:

```javascript
bot.command({
  name: 'charCount',
  code: `
  $charCount[aoi.js is one of the simplest and easiest ways to create your own Discord Bot]
  `
});
```
