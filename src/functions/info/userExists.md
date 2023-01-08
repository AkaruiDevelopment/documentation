---
title: $userExists 
description: $userExists will check if a given user exists.
id: userExists
---

`$userExists` will check if a given user exists.

## Usage

```php
$userExists[userID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| userID?    | integer  | user ID                             | no      |


## Example

This will return either `true` or `false` depending on if the user exists, in this example below it will return `true` as you exist as Discord user:

```javascript
bot.command({
  name: 'userExists',
  code: `
  $userExists[$authorID]
  `
});
```
