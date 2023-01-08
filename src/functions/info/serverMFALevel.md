---
title: $serverMFALevel 
description: $serverMFALevel will return the guild's MFA Level.
id: serverMFALevel
---

`$serverMFALevel` will return the guild's MFA Level.

## Usage

```php
$serverMFALevel[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |

| Type     |         |
|----------|---------|
| 0  | guild has no MFA/2FA requirement for moderation actions |
| 1  | guild has a 2FA requirement for moderation actions      |

## Example

This will return the guild's MFA Level:

```javascript
bot.command({
  name: 'serverMFALevel',
  code: `
  $serverMFALevel[$guildID]
  `
});
```
