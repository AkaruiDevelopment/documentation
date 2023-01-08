---
title: $channelOverwrites 
description: $channelOverwrites will return the given channel's overwrites.
id: channelOverwrites
---

`$channelOverwrites` will return the given channel's overwrites.

## Usage

```php
$channelOverwrites[channelID?;response?;sep?]
```

## Parameters 


| Field      | Type    | Description                                                         | Required |
| ---------- | ------- | ------------------------------------------------------------------- | :------: |
| channelID? | integer | channel ID of the channel you want the channel overwrites of        |    no    |
| response?  | string  | the format the channel overwrites will be returned in               |    no    |
| sep?       | string  | the seperator to split the channel overwrites if there are multiple |    no    |


|    Type     | Output                         |
| :---------: | ------------------------------ |
| `{mention}` | Mentions the role or user      |
|  `{type}`   | Returns the type, user or role |
|  `{allow}`  | The granted permissions        |
|  `{deny}`   | The denied permissions         |


## Example

This will return the channel overwrites of the channel where you execute the command in:

```javascript
bot.command({
  name: 'channelOverwrites',
  code: `
  $channelOverwrites[$channelID;{mention} {type} {allow} {deny};, ]
  `
});
```