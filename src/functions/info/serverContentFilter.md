---
title: $serverContentFilter 
description: $serverContentFilter will return the guild's content filter level.
id: serverContentFilter
---

`$serverContentFilter` will return the guild's content filter level.

## Usage

```php
$serverContentFilter[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | yes      |


| Type     |         | 
|-----------|---------|
| 0    | Disabled  |
| 1    | Medium  |
| 2    | High  |


## Example

This will return the content filter level of a specific guild:

```javascript
bot.command({
  name: 'serverContentFilter',
  code: `
  $serverContentFilter[$guildID]
  `
});
```
