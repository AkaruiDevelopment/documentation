---
title: $isChannelManageable 
description: $isChannelManageable will check if the channel is manageable or not.
id: isChannelManageable
---

`$isChannelManageable` will check if the channel is manageable or not.

## Usage

```php
$isChannelManageable[channelID?]
```

## Parameters 


| Field      | Type    | Description                                                   | Required |
| ---------- | ------- | ------------------------------------------------------------- | -------- |
| channelID? | integer | channel id where to check if the channel is manageable or not | no       |


## Example

This will return `true` or `false` depending on if the channel you're executing the command in is manageable:

```javascript
bot.command({
  name: 'isChannelManageable',
  code: `
  $isChannelManageable[$channelID]
  `
});
```
