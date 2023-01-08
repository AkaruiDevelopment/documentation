---
title: $mentionedUsersCount 
description: $mentionedUsersCount will return the amount of user mentions within a message.
id: mentionedUsersCount
---

`$mentionedUsersCount` will return the amount of user mentions within a message.

## Usage

```php
$mentionedUsersCount
```

## Example

This will return the amount of user mentions in the given text:

```javascript
bot.command({
  name: 'mentionedUsersCount',
  code: `
  Amount of user mentions: $mentionedUsersCount
`
});
```
