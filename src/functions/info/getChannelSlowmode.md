---
title: $getChannelSlowmode 
description: $getChannelSlowmode will return a channel's slowmode in seconds.
id: getChannelSlowmode
---

`$getChannelSlowmode` will return a channel's slowmode in seconds.

## Usage

```php
$getChannelSlowmode[channelID?]
```

## Parameters 


| Field      | Type    | Description                                                      | Required |
| ---------- | ------- | ---------------------------------------------------------------- | -------- |
| channelID? | integer | channel ID of the channel where you want the channel slowmode of | no       |


## Example

This will return the slowmode of the channel where you execute the command in:

```javascript
bot.command({
  name: 'getChannelSlowmode',
  code: `
  The current channel slowmode is: $getChannelSlowmode[$channelID] seconds!
  `
});
```