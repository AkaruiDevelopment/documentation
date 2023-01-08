---
title: $isVoice 
description: $isVoice will check if the given channel is a voice channel or not.
id: isVoice
---

`$isVoice` will check if the given channel is a voice channel or not.

## Usage

```php
$isVoice[channelID]
```

## Parameters 


| Field      | Type    | Description                              | Required |
| ---------- | ------- | ---------------------------------------- | -------- |
| channelID? | integer | ID of the channel that you want to check | no       |


## Example

This will return either `true` or `false` depending on what you use as argument:

```javascript
bot.command({
  name: 'isVoice',
  code: `
  $isVoice[$channelID]
  `
});
```