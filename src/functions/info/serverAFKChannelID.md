---
title: $serverAFKChannelID 
description: $serverAFKChannelID will return a guild's AFK voice channel.
id: serverAFKChannelID
---

`$serverAFKChannelID` will return a guild's AFK voice channel

## Usage

```php
$serverAFKChannelID[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| guildID?    | integer  | guild ID                             | yes      |


## Example

This will return the AFK voice channel of your guild:

```javascript
bot.command({
  name: 'serverAFKChannelID',
  code: `
  $serverAFKChannelID
  `
});
```
