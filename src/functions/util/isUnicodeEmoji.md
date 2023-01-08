---
title: $isUnicodeEmoji 
description: $isUnicodeEmoji will check if the given emoji is an unicode emoji.
id: isUnicodeEmoji
---

`$isUnicodeEmoji` will check if the given emoji is an unicode emoji.

## Usage

```php
$isUnicodeEmoji[emoji]
```

## Parameters 


| Field | Type   | Description   | Required |
| ----- | ------ | ------------- | -------- |
| emoji | string | unicode emoji | yes      |


## Example

This will return `true` as "🤓" is an valid unicode emoji:

```javascript
bot.command({
  name: 'isUnicodeEmoji',
  code: `
  $isUnicodeEmoji[🤓]
  `
});
```
