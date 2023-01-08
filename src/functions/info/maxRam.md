---
title: $maxRam 
description: $maxRam will return the bot's maximum amount of Ram.
id: maxRam
---

`$maxRam` will return the bot's maximum amount of Ram.

## Usage

```php
$maxRam
```

## Example

This will your bot's maximum amount of available Ram:

```javascript
bot.command({
  name: 'maxRam',
  code: `
  $maxRam
  `
});
```
