---
title: $readyTimestamp 
description: $readyTimestamp will return the timestamp of when the bot was ready.
id: argsCheck
---

`$argsSlice` will return the timestamp of when the bot was ready.

## Usage

```php
$readyTimestamp
```

## Example

This will return the last time your bot when online:

```javascript
bot.command({
  name: 'readyTimestamp',
  code: `
  $readyTimestamp
  `
});
```
