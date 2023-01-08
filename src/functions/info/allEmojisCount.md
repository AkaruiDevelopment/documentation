---
title: $allEmojisCount 
description: $allEmojisCount will return the amount of emojis of a given type.
id: allEmojisCount
---

`$allEmojisCount` will return the amount of emojis of a given type.

## Usage

```php
$allEmojisCount[type?]
```

## Parameters 


| Field | Type   | Description                 | Required |
| ----- | ------ | --------------------------- | -------- |
| type? | string | type you want the amount of | no       |


| Emoji Type      |          |
| --------------- | -------- |
| Animated Emojis | animated |
| Stable Emojis   | normal   |


## Example

This will return the amount of emojis in your guild:

```javascript
bot.command({
  name: 'allEmojisCount',
  code: `
  $allEmojisCount
  `
});
```