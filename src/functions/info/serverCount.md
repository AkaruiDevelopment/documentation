---
title: $serverCount 
description: $serverCount will return the amount of servers where your bot is in.
id: serverCount
---

`$serverCount` will return the amount of servers where your bot is in.

## Usage

```php
$serverCount
```

## Example

This will return the amount of servers your bot is in:

```javascript
bot.command({
  name: 'serverCount',
  code: `
  I'm in $serverCount servers!
  `
});
```
