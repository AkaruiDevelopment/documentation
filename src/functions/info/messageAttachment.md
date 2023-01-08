---
title: $messageAttachment 
description: $messageAttachment will return a message attachment depending on the given index.
id: message
---

`$messageAttachment` will return a message attachment depending on the given index.

## Usage

```php
$messageAttachment[index?]
```

## Parameters 


| Field  | Type    | Description                                              | Required |
| ------ | ------- | -------------------------------------------------------- | :------: |
| index? | integer | which message attachment to return, <br> **1** - default |    no    |


## Example

This will return your given attachment:

```javascript
bot.command({
  name: 'messageAttachment',
  code: `
  You had the following attachment in your message: $messageAttachment
  `
});
```
