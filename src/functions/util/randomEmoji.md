---
title: $randomEmoji 
description: $randomEmoji will return a random emoji ID.
id: randomEmoji
---

`$randomEmoji` will return a random emoji ID.

## Usage

```php
$randomEmoji
```

## Example

This will return a random emoji ID of your guild:

```javascript
bot.command({
  name: 'randomEmoji',
  code: `
  $randomEmoji
  `
});
```
