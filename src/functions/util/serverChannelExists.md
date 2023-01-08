---
title: $serverChannelExists 
description: $serverChannelExists will check if the given server channel exists.
id: serverChannelExists
---

`$serverChannelExists` will check if the given server channel exists.

## Usage

```php
$serverChannelExists[channel;guildID?]
```

## Parameters 


| Field   | Type    | Description                                        | Required |
| ------- | ------- | -------------------------------------------------- | -------- |
| channel | string  | channel ID or name of the server channel           | yes      |
| guildId | integer | id of the guild where the server channel exists in | yes      |


## Example

This will check if a server channel with the name `rules` exists, alternatively you could use the channel ID instead:

```javascript
bot.command({
  name: 'serverChannelExists',
  code: `
  $serverChannelExists[rules]
  `
});
```
