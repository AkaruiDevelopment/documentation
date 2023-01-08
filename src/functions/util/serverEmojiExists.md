---
title: $serverEmojiExists 
description: $serverEmojiExists will check if the given emoji exists in the given guild.
id: serverEmojiExists
---

`$serverEmojiExists` will check if the given emoji exists in the given guild.

## Usage

```php
$serverEmojiExists[emoji;guildId?]
```

## Parameters 


| Field    | Type    | Description                                  | Required |
| -------- | ------- | -------------------------------------------- | -------- |
| emoji    | string  | emoji you want to check if it exists         | yes      |
| guildId? | integer | guild id of the guild where the emoji exists | no       |

### Please note that your bot has to be present in the guild where the emoji is in.

## Example

This will return `true` as the ![emoji](https://cdn.discordapp.com/emojis/1003365344724910191.webp?size=16&quality=lossless) emoji exists:

```javascript
bot.command({
  name: 'serverEmojiExists',
  code: `
  $serverEmojiExists[<:LerefMoney:1003365344724910191>;$guildID]
  `
});
```
