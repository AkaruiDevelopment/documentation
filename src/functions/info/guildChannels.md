---
title: $guildChannels 
description: $guildChannels will return all channels of a specific guild.
id: guildChannels
---

`$guildChannels` will return all channels of a specific guild.

## Usage

```php
$guildChannels[guildID?;option?;sep?]
```

## Parameters 


| Field    | Type    | Description                                        | Required  |
|----------|---------|----------------------------------------------------| :-------: |
| guildID? | integer | the ID of the guild                                | no        |
| option?  | string  | the option on how to return the channel <br> 1. **name** (default) <br> 2. **id** <br> 3. **mention**        | no       |
| sep?     | string  | seperator to seperate multiple arguments           | no        |


## Example

This will return all channels of your guild:

```javascript
bot.command({
  name: 'guildChannels',
  code: `
  $guildChannels[$guildID;mention;, ]
  `
});
```
