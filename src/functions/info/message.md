---
title: $message 
description: $message will return given arguments of a message.
id: message
---

`$message` will return given arguments of a message.

## Usage

```php
$message[index?]
```

## Parameters 


| Field  | Type    | Description                                                   | Required |
| ------ | ------- | ------------------------------------------------------------- | :------: |
| index? | integer | which message to return, leave empty to return every argument |    no    |


## Example

This will return your given message:

```javascript
bot.command({
  name: 'message',
  code: `
  You've said: "$message"
  `
});
```
