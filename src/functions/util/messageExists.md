---
title: $messageExists 
description: $messageExists will check if a specific message exists.
id: messageExists
---

`$messageExists` will check if a specific message exists.

## Usage

```php
$messageExists[messageid;channelid?]
```

## Parameters 


| Field      | Type    | Description                                 | Required |
| ---------- | ------- | ------------------------------------------- | -------- |
| messageid  | integer | the id of the message                       | yes      |
| channelid? | integer | the channel id where the message is located | no       |


## Example

This will return `false` as the message doesn't exist in the given channel:

```javascript
bot.command({
  name: 'messageExists',
  code: `
  $messageExists[1058998634823299143;$channelID]
  `
});
```
