---
title: $mentioned 
description: $mentioned will return the ID of an user of the mention.
id: mentioned
---

`$mentioned` will return the ID of an user of the mention.

## Usage

```php
$mentioned[index;returnSelf?]
```

## Parameters 


| Field       | Type   | Description                                  | Required |
| ----------- | ------ | -------------------------------------------- | -------- |
| index       | number | the index of the argument                    | yes      |
| returnSelf? | string | return the author's id if user was not found | no       |


## Example

This will return the ID of the **first** mention if you attempt to mention someone in this command, or else it will return your ID:

```javascript
bot.command({
  name: 'mentioned',
  code: `
  $mentioned[1;yes]
  `
});
```
