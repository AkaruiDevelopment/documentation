---
title: $messageSlice 
description: $messageSlice will slice a message.
id: messageSlice
---

`$messageSlice` will slice a message.

## Usage

```php
$messageSlice[from;to?]
```

## Parameters 


| Field | Type   | Description                               | Required |
| ----- | ------ | ----------------------------------------- | -------- |
| from  | number | starting point where to slice the message | yes      |
| to?   | number | ending point where slicing ends           | no       |


## Example

This will slice the message from the first character to the fifth character:

```javascript
bot.command({
  name: 'messageSlice',
  code: `
  $messageSlide[1;5]
  `
});
```
