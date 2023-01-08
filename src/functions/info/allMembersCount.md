---
title: $allMembersCount 
description: $allMembersCount will return the amount of members in your guild.
id: allMembersCount
---

`$allMembersCount` will return the amount of members in your guild.

## Usage

```php
$allMembersCount
```

## Example

This will return the amount of members in your guild:

```javascript
bot.command({
  name: 'allMembersCount',
  code: `
  $allMembersCount
  `
});
```