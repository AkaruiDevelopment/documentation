---
title: $authorID 
description: $authorID will return user ID of who executed the command.
id: authorID
---

`$authorID` will return user ID of who executed the command.

## Usage

```php
$authorID
```

## Example

This will return your user ID:

```javascript
bot.command({
  name: 'authorID',
  code: `
  $authorID
  `
});
```