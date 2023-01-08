---
title: $findServerChannel 
description: $findServerChannel will search a server channel within a guild.
id: findServerChannel
---

`$findServerChannel` will search a server channel within a guild.

## Usage

```php
$findServerChannel[channelResolver;returnSelf?;guildID?]
```

## Parameters 


| Field           | Type    | Description                                                             | Required |
| --------------- | ------- | ----------------------------------------------------------------------- | -------- |
| channelResolver | string  | name of the channel you are trying to find                              | yes      |
| returnSelf?     | string  | return the channel where the command got executed in when nothing found | no       |
| guildID?        | integer | guild ID where the channel is present in                                | no       |


## Example

This will return the channel ID of an channel called `#rules`

```javascript
bot.command({
  name: 'findServerChannel',
  code: `
  $findServerChannel[rules;no;$guildID]
  `
});
```
