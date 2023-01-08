---
title: $memberJoinedDate 
description: $memberJoinedDate will return a members join date in MS.
id: memberJoinedDate
---

`$memberJoinedDate` will return a members join date in MS.

## Usage

```php
$memberJoinedDate[userID?;guildID?]
```

## Parameters 


| Field    | Type    | Description                                            | Required |
| -------- | ------- | ------------------------------------------------------ | :------: |
| userID?  | integer | the ID of the member                                   |    no    |
| guildID? | integer | the ID of the guild                                    |    no    |


## Example

This will return your join date in MS:

```javascript
bot.command({
  name: 'memberJoinPosition',
  code: `
  $memberJoinedDate[$authorID;$guildID]
  `
});
```
