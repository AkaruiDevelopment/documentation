---
title: $getBanReason 
description: $getBanReason will return a ban reason of an specific user.
id: getBanReason
---

`$getBanReason` will return a ban reason of an specific user.

## Usage

```php
$getBanReason[guildID?;userID?]
```

## Parameters 


| Field    | Type    | Description                                                 | Required |
| -------- | ------- | ----------------------------------------------------------- | -------- |
| guildID? | integer | the guild ID                                                | no       |
| userID?  | integer | the user ID of the user you want to check the ban reason of | no       |


#### Please note that your bot requires `VIEW_AUDIT_LOG` permissions

## Example

This will return the ban reason of whoever you'd like:

```javascript
bot.command({
  name: 'getBanReason',
  code: `
  $getBanReason[$guildID;userID] //make sure to replace "userID" with an actual user ID
  `
});
```