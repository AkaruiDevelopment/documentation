---
title: $channelName 
description: $channelName will return the channel name of the given channel.
id: channelName
---

`$channelName` will return the channel name of the given channel.

## Usage

```php
$channelName[channelID?]
```

## Parameters 


| Field      | Type    | Description                                            | Required |
| ---------- | ------- | ------------------------------------------------------ | :------: |
| channelID? | integer | channel ID of the channel you want the channel name of |    no    |


## Example

This will return the channel name of the channel where you executed the command in:

```javascript
bot.command({
  name: 'channelName',
  code: `
  $channelName[$channelID]
  `
});
```