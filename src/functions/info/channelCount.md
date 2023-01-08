---
title: $allChannelsCount 
description: $allChannelsCount will return the amount of channels of a given type.
id: allChannelsCount
---

`$allChannelsCount` will return the amount of channels of a given type.

## Usage

```php
$channelCount[guildID?;type?]
```

## Parameters 


| Field    | Type    | Description                                                    | Required |
| -------- | ------- | -------------------------------------------------------------- | :------: |
| guildID? | integer | guild id of the guild where you want the amount of channels of |    no    |
| type?    | string  | type you want the amount of                                    |    no    |


| Channel Type         |                |
| -------------------- | -------------- |
| Text Channel         | Text           |
| Voice Channel        | Voice          |
| Category             | Category       |
| Stage Channel        | Stage          |
| Private Thread       | PrivateThread  |
| Public Thread        | PublicThread   |
| Announcement Thread  | NewsThread     |
| Announcement Channel | News           |
| Home                 | GuildDirectory |
| NSFW Channel         | NSFW           |
| all types            | all            |


## Example

This will return the amount of Voice Channels in your guild:

```javascript
bot.command({
  name: 'channelCount',
  code: `
  $channelCount[$guildID;Voice]
  `
});
```