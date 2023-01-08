---
title: $mentionedChannels
description: $mentionedChannels will return the ID of a channel retrieved from the mention.
id: mentionedChannels
---

`$mentionedChannels` will return the ID of a channel retrieved from the mention.

## Usage

```php
$mentionedChannels[index;returnSelf?]
```

## Parameters 


| Field       | Type   | Description                                                                               | Required |
| ----------- | ------ | ----------------------------------------------------------------------------------------- | -------- |
| index       | number | the index of the argument                                                                 | yes      |
| returnSelf? | string | return the id of the channel where the command was executed in when channel was not found | no       |


## Example

This will return the ID of the **first** mention if you attempt to mention any channel in this command, or else it will return the channel ID of the channel where the command was executed in:

```javascript
bot.command({
  name: 'mentionedChannels',
  code: `
  $mentionedChannels[1;yes]
  `
});
```
