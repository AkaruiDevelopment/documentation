---
title: $status 
description: $status will a user's presence.
id: status
---

`$status` will a user's presence.

## Usage

```php
$status[userId?;guildId?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| userId?    | integer  | user ID                             | no      |
| guildId?    | integer  | guild ID                             | no      |


## Example

This will either return `idle`, `online`, `invisible` or `dnd` depending on your current presence:

```javascript
bot.command({
  name: 'status',
  code: `
  $status[$authorID;$guildID]
  `
});
```
