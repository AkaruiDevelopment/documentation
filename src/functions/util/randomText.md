---
title: $randomText 
description: $randomText will return a random word out of the given query
id: randomText
---

`$randomText` will return a random word out of the given query

## Usage

```php
$randomText[text;text;...]
```

## Parameters 


| Field | Type   | Description                              | Required |
| ----- | ------ | ---------------------------------------- | -------- |
| text  | string | any words you want to be chosen randomly | yes      |


## Example

This will return a random text out of `Hello, Bye, Goodnight, See you`:

```javascript
bot.command({
  name: 'randomText',
  code: `
  $randomText[Hello;Bye;Goodnight;See you]
  `
});
```
