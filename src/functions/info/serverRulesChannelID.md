---
title: $serverRulesChannelID 
description: $serverRulesChannelID will return a guild's set rules channel ID.
id: serverRulesChannelID
---

`$serverRulesChannelID` will return a guild's set rules channel ID.

## Usage

```php
$serverRulesChannelID[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?  | integer | guild ID                                           | no       |


## Example

This will return the ID of the server's rules channel (community servers only):

```javascript
bot.command({
  name: 'serverRulesChannelID',
  code: `
  $serverRulesChannelID[$guildID]
  `
});
```
