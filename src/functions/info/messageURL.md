---
title: $messageURL 
description: $messageURL will return the URL of a given message.
id: messageURL
---

`$messageURL` will return the URL of a given message.

## Usage

```php
$messageURL[messageID?;channelID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------|:----------:|
| messageID?      | integer  | id of the message                             | no      |
| channelID?      | integer  | channel ID of where the message is located in                             | no      |


## Example

This will return the message URL of the message which executed the command:

```javascript
bot.command({
  name: 'messageURL',
  code: `
  $messageURL[$messageID;$channelID]
  `
});
```
