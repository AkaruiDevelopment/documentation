---
title: $maximumMembers 
description: $maximumMembers will return the maximal amount of members a guild can have.
id: maximumMembers
---

`$maximumMembers` will return the maximal amount of members a guild can have.

## Usage

```php
$maximumMembers[guildID?]
```

## Parameters 


| Field    | Type    | Description         | Required |
| -------- | ------- | ------------------- | :------: |
| guildID? | integer | the ID of the guild |    no    |


## Example

This will return the maximum of members you can have in your guild:

```javascript
bot.command({
  name: 'maximumMembers',
  code: `
  You can have: $maximumMembers[$guildID] Members in this guild!
  `
});
```
