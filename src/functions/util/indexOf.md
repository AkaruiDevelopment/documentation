---
title: $indexOf 
description: $indexOf will return the index of the given character.
id: indexOf
---

`$indexOf` will return the index of the given character.

## Usage

```php
$indexOf[string;char]
```

## Parameters 


| Field  | Type   | Description                                    | Required |
| ------ | ------ | ---------------------------------------------- | -------- |
| string | string | the text the bot will be checking the index of | yes      |
| char   | string | the character the bot will be checking for     | yes      |


## Example

This will return `8` as it's the first occuring position of the character `w`:

```javascript
bot.command({
  name: 'indexOf',
  code: `
  $indexOf[Hello, what is wrong with you?;w]
  `
});
```
