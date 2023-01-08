---
title: $nonEscape 
description: $nonEscape will stop escaping special characters.
id: nonEscape
---

`$nonEscape` will stop escaping special characters.

## Usage

```php
$nonEscape[message]
```

## Parameters 


| Field   | Type   | Description                      | Required |
| ------- | ------ | -------------------------------- | -------- |
| message | string | text you dont want to be escaped | yes      |


## Example

This will stop from escaping certain characters:

```javascript
bot.command({
  name: 'nonEscape',
  code: `
  $nonEscape[Hello [;)]]
  `
});
```
