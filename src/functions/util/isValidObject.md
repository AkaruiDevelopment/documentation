---
title: $isValidObject 
description: $isValidObject checks if the given json is a valid object.
id: isValidObject
---

`$isValidObject` checks if the given json is a valid object.

## Usage

```php
$isValidObject[json]
```

## Parameters 


| Field | Type   | Description | Required |
| ----- | ------ | ----------- | -------- |
| json  | string | json object | yes      |

### This function will only work if it's a JSON Object

## Example

This will return `true` as the given object is an valid json object:

```javascript
bot.command({
  name: 'isValidObject',
  code: `
  $isValidObject[{"name":"Leref", "aoijs":"nice"}]
  `
});
```
