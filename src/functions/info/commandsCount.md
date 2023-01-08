---
title: $commandsCount 
description: $commandsCount will return the amount of commands.
id: commandsCount
---

`$commandsCount` will return the amount of commands.


## Usage

```php
$commandsCount
```

## Example

This will return the the amount of your commands:

```javascript
bot.command({
  name: 'commandsCount',
  code: `
  $commandsCount
  `
});
```