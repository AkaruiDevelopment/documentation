---
title: $mentionedRoles 
description: $mentionedRoles will return the ID of a role retrieved from a message, this works similar as `$mentioned`.
id: mentionedRoles
---

`$mentionedRoles` will return the ID of a role retrieved from a message.

## Usage

```php
$mentionedRoles[index]
```

## Parameters 


| Field | Type   | Description               | Required |
| ----- | ------ | ------------------------- | -------- |
| index | number | the index of the argument | yes      |

## Example

This will return the ID of the **first** role mention if you attempt to mention any role in this command:

```javascript
bot.command({
  name: 'mentionedRoles',
  code: `
  $mentionedRoles[1]
  `
});
```
