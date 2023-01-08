---
title: $membersCount 
description: $membersCount will return a guild's member count.
id: membersCount
---

`$membersCount` will return a guild's member count.

## Usage

```php
$membersCount[guildID?;presence?;countBot?]
```

## Parameters 


| Field     | Type    | Description                                                                                                                 | Required |
| --------- | ------- | --------------------------------------------------------------------------------------------------------------------------- | :------: |
| guildID?  | integer | the ID of the guild                                                                                                         |    no    |
| presence? | string  | the presence of the users <br> 1. **all** (default) <br> 2. **dnd** <br> 3. **idle** <br> 4. **offline** <br> 5. **online** |    no    |
| countBot? | string  | count bots? <br> 1. **yes** (default) <br> 2. **no**                                                                                                       |    no    |


## Example

This will return the amount of offline users (including bots) in your guild:

```javascript
bot.command({
  name: 'membersCount',
  code: `
  $membersCount[$guildID;offline;yes]
  `
});
```
