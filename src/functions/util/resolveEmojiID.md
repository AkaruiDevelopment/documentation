---
title: $resolveEmojiID 
description: $resolveEmojiID will resolve a certain emoji.
id: resolveEmojiID
---

`$resolveEmojiID` will resolve a certain emoji.

## Usage

```php
$resolveEmojiID[emoji]
```

## Parameters 


| Field | Type   | Description | Required |
| ----- | ------ | ----------- | -------- |
| emoji | string | emoji name  | yes      |

### Please note that your bot has to be present in the guild where the emoji is in.


## Example

This will return `<:LerefMoney:1003365344724910191>`:

```javascript
bot.command({
  name: 'resolveEmojiID',
  code: `
  $resolveEmojiID[LerefMoney]
  `
});
```