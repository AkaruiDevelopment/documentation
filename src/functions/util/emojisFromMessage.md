---
title: $emojisFromMessage 
description: $emojisFromMessage will retrieve all emojis given in a message.
id: emojisFromMessage
---

`$emojisFromMessage` returns all emojis in a given message.

## Usage

```php
$emojisFromMessage
```
### Please note that your bot has to be present in the guild where the emoji is in.

## Example

This will return any emojis you give as argument:

```javascript
bot.command({
  name: 'emojisFromMessage',
  code: `
$emojisFromMessage
  `
});
```
