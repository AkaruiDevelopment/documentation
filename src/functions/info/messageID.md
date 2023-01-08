---
title: $messageID
description: $messageID will return the message ID.
id: messageID
---

`$messageID` will return the message ID.

## Usage

```php
$messageID
```


## Example

This will return the message ID of the message with which you executed the command:

```javascript
bot.command({
  name: 'messageID',
  code: `
  The message ID of your the message you just sent is: "$messageID"
  `
});
```
