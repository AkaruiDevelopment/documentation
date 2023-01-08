---
title: $findRoles 
description: $findRoles will return all matching roles depending on the given query.
id: findRoles
---

`$findRoles` will return all matching roles depending on the given query.

## Usage

```php
$findRoles[query;limit?;type?;res?]
```

## Parameters 


| Field  | Type   | Description                                     | Required |
| ------ | ------ | ----------------------------------------------- | -------- |
| query  | string | name of the role you want to find               | yes      |
| limit? | number | the maximum amount of roles the bot will return | no       |
| type?  | string | type of the search query                        | no       |
| res?   | string | formatting for the output                       | no       |

### Parameters for the `res` argument
* {position} -> returns the position
* {id} -> returns the role ID
* {username} -> returns the role name


## Example

This will return all roles which are named `Owner`:

```javascript
bot.command({
  name: 'findRoles',
  code: `
  $findRoles[Owner;5;startsWith;{position}) {username}: {id}]
  `
});
```
