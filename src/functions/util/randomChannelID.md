---
title: $randomChannelID 
description: $randomChannelID will return a random channel ID of all guilds or of a specific guild.
id: randomChannelID
---

`$randomChannelID` will return a random channel ID of all guilds or of a specific guild.

## Usage

```php
$randomChannelID[guildID/global?;type?]
```

## Parameters 


| Field           | Type    | Description               | Required |
| --------------- | ------- | ------------------------- | -------- |
| guildID/global? | integer | guild ID or global search | no       |
| type?           | string  | channel type              | no       |

<details open>
  <summary> <h3> Channel Types </h3></summary>

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
| all types            | all            |

#### Note: all channel types are **case-sensitive**.

</details>

## Example

This will return a random channel ID of your guild:

```javascript
bot.command({
  name: 'randomChannelID',
  code: `
  <#$randomChannelID[$guildID;all]>
  `
});
```
