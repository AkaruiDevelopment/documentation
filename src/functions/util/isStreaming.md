---
title: $isStreaming 
description: $isStreaming will check if one user is streaming in a voice channel.
id: isStreaming
---

`$isStreaming` will check if one user is streaming in a voice channel.

## Usage

```php
$isStreaming[userid?;guildid?]
```

## Parameters 


| Field    | Type    | Description                                                    | Required |
| -------- | ------- | -------------------------------------------------------------- | -------- |
| userid?  | integer | the user id of the user you want to check if they're streaming | no       |
| guildid? | integer | the guild id of where they're streaming in                     | no       |


## Example

This will return either `true` or `false` depending on if you're streaming (voice channel) or not:

```javascript
bot.command({
  name: 'isStreaming',
  code: `
  $isStreaming[$authorid;$guildid]
  `
});
```
