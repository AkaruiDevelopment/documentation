---
title: $activity 
description: $activity will return a users current voice channel activity.
id: activity
---

`$activity` will return a users current activity.

## Usage

```php
$activity[id?;guildID?]
```

## Parameters 


| Field  | Type    | Description | Required |
| ------ | ------- | ----------- | -------- |
| id?    | integer | user id     | yes      |
| guild? | integer | guild id    | no       |


## Example

This will return your current voice channel Activity:

```javascript
bot.command({
  name: 'activity',
  code: `
  $activity[$authorID;$guildID]
  `
});
```