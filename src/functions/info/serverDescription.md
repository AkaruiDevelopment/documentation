---
title: $serverDescription 
description: $serverDescription will return the guild's description.
id: serverDescription
---

`$serverDescription` will return the guild's description.

## Usage

```php
$serverDescription[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | no      |


## Example

This will return the description of a specific guild:

```javascript
bot.command({
  name: 'serverDescription',
  code: `
  $serverDescription[$guildID]
  `
});
```
