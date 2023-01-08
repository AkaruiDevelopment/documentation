---
title: $randomGuildID 
description: $randomGuildID will return a random guild ID.
id: randomChannelID
---

`$randomGuildID` will return a random guild ID.

## Usage

```php
$randomGuildID
```

## Example

This will return a random server name using the `$randomGuildID` and `$serverName` function:

```javascript
bot.command({
  name: 'randomGuildID',
  code: `
  $serverName[$randomGuildID]
  `
});
```
