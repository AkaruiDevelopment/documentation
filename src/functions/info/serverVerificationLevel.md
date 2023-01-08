---
title: $serverVerificationLevel 
description: $serverVerificationLevel will return the guild's verification level.
id: serverVerificationLevel
---

`$serverVerificationLevel` will return the guild's verification level.

## Usage

```php
$serverVerificationLevel[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                                        | no       |

| Type     |         |
|----------|---------|
| 0  | None |
| 1  | Low     |
| 2  | Medium    |
| 3  | High     |
| 4  | Highest   |


## Example

This will return the guild's verification Level:

```javascript
bot.command({
  name: 'serverVerificationLevel',
  code: `
  $serverVerificationLevel[$guildID]
  `
});
```
