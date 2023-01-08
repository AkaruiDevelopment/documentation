---
title: $findMember 
description: $findMember will find a specific member in a specific guild by their name.
id: findMember
---

`$findMember` will find a specific member in a specific guild.

## Usage

```php
$findMember[user;returnSelf?;guildID?]
```

## Parameters 


| Field       | Type    | Description                                  | Required |
| ----------- | ------- | -------------------------------------------- | -------- |
| user        | string  | user you want to find                        | yes      |
| returnSelf? | string  | return the author's id if user was not found | no       |
| guildID?    | integer | guild ID where the user is present in        | no       |


## Example

This will return your ID as `Leref` was not found in the given guild:

```javascript
bot.command({
  name: 'findMember',
  code: `
  $findMember[Leref;yes;$guildID]
  `
});
```
