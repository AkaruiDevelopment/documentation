---
title: $hoistedRole 
description: $hoistedRole will return the highest hoisted role of an user.
id: hoistedRole
---

`$hoistedRole` will return the highest hoisted role of an user.

## Usage

```php
$hoistedRole[userID?;guildID?;option?]
```

## Parameters 


| Field    | Type    | Description                                                                                         | Required |
| -------- | ------- | --------------------------------------------------------------------------------------------------- | :------: |
| userID?  | integer | the ID of the user                                                                                  |    no    |
| guildID? | integer | the ID of the guild                                                                                 |    no    |
| option?  | string  | the option on how to return the role <br> 1. **name** <br> 2. **id**  (default) <br> 3. **mention** |    no    |


## Example

This will return the name of your highest hoisted role:

```javascript
bot.command({
  name: 'hoistedRole',
  code: `
  $hoistedRole[$authorID;$guildID;name]
  `
});
```
