---
title: $reactionCount 
description: $reactionCount will return the amount of users who reacted to a specific emoji.
id: reactionCount
---

`$reactionCount` will return the amount of users who reacted to a specific emoji.

## Usage

```php
$reactionCount[channelID;messageID;emoji]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :--------: |
| channelID      | integer  | the channel ID                             | yes      |
| messageID     | integer  | the message ID          | yes       |
| emoji        | string  | the emoji its reaction count will be returned of                | yes      |


## Example

This will return the amount of reactions on your message with which you executed the command, will most likely return `1` due to the bot being the only one who reacted to it:

```javascript
bot.command({
  name: 'reactionCount',
  code: `
There are: $reactionCount[$channelID;$messageID;😫] reactions!
$addCmdReactions[😫]
`
});
```
