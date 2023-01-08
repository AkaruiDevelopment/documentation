---
title: $platform 
description: $platform will return the platform which the user is using Discord with.
id: platform
---

`$platform` will return the platform which the user is using Discord with.

## Usage

```php
$platform[userID?;guildID?;sep?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------|----------|
| userID?      | integer  | ID of the user                             | no      |
| guildID?     | integer  | the guild ID          | no       |
| sep?        | string  | the seperator to split multiple arguments                   | no      |


## Example

This will return your platform you're using Discord on:

```javascript
bot.command({
  name: 'platform',
  code: `
  $platform[$authorID;$guildID;, ]
  `
});
```
