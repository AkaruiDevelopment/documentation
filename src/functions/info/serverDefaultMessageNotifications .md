---
title: $serverDefaultMessageNotifications  
description: $serverDefaultMessageNotifications will return given guild's default message notification type.
id: serverDefaultMessageNotifications 
---

`$serverDefaultMessageNotifications ` will return given guild's default message notification type.

## Usage

```php
$serverDefaultMessageNotifications[guild?]
```

## Parameters 


| Field    | Type    | Description                                                | Required |
| -------- | ------- | ---------------------------------------------------------- | :------: |
| guildID? | integer | guild id you want the default message notification type of |    no    |


## Example

This will return the guild's default message notification type:

```javascript
bot.command({
  name: 'serverDefaultMessageNotifications',
  code: `
  $serverDefaultMessageNotifications
  `
});
```