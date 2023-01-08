---
title: $findUser 
description: $findUser will attempt to find a user which is matching with the given query.
id: findUser
---

`$findUser` will attempt to find a user which is matching with the given query.

## Usage

```php
$findUser[userResolver;returnSelf?]
```

## Parameters 


| Field        | Type   | Description                                                                          | Required |
| ------------ | ------ | ------------------------------------------------------------------------------------ | -------- |
| userResolver | string | query which is used to find the user                                                 | yes      |
| returnSelf?  | string | will return the user id of the user who executed the command when user was not found | no       |


## Example

This will search for a user called Ferel, if it wont find the user then it'll return your user ID:

```javascript
bot.command({
  name: 'findUser',
  code: `
  $findUser[Ferel;yes]
  `
});
```
