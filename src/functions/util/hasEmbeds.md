---
title: $hasEmbeds 
description: $hasEmbeds will check if there are embeds attached to the message.
id: hasEmbeds
---

`$hasEmbeds` will check if there are embeds attached to the message.

## Usage

```php
$hasEmbeds[messageID;channelID]
```

## Parameters 

| Field     | Type    | Description                                             | Required |
| --------- | ------- | ------------------------------------------------------- | -------- |
| messageID | integer | message ID of the embed                                 | yes      |
| channelID | integer | channel ID of the channel where the embed is present in | yes      |


## Example

This will return `false` as there are no embeds attached to your message:

```javascript
bot.command({
  name: 'hasEmbeds',
  code: `
  $hasEmbeds[$messageID;$channelID]
  `
});
```
