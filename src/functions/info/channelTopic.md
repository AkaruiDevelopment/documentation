---
title: $channelTopic 
description: $channelTopic will return the given channel's topic.
id: channelTopic
---

`$channelTopic` will return the given channel's topic.

## Usage

```php
$channelTopic[channelID?]
```

## Parameters 


| Field      | Type    | Description                                             | Required |
| ---------- | ------- | ------------------------------------------------------- | :------: |
| channelID? | integer | channel ID of the channel you want the channel topic of |    no    |


## Example

This will return the channel topic of the channel where you execute the command in:

```javascript
bot.command({
  name: 'channelTopic',
  code: `
  $channelTopic[$channelID]
  `
});
```