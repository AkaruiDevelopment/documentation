---
title: $isVideoOn 
description: $isVideoOn checks if the given user has their video on in a voice channel.
id: isVideoOn
---

`$isVideoOn` checks if the given user has their video on in a voice channel.

## Usage

```php
$isVideoOn[userid?;guildid?]
```

## Parameters 


| Field    | Type    | Description                                                             | Required |
| -------- | ------- | ----------------------------------------------------------------------- | -------- |
| userid?  | integer | user id of the user who turned video on                                 | no       |
| guildid? | integer | the guild ID of the guild you want to check if they have their video on | no       |


## Example

This will check if you're currently using the video feature in a voice channel:

```javascript
bot.command({
  name: 'isVideoOn',
  code: `
  $isVideoOn[$authorid;$guildid]
  `
});
```
