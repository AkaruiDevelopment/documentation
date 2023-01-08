---
title: $toUpperCase 
description: $toUpperCase will change the given text from lowercase to uppercase.
id: toUpperCase
---

`$toUpperCase` will change the given text from lowercase to uppercase.

## Usage

```php
$toUpperCase[text]
```

## Parameters 


| Field | Type   | Description | Required |
| ----- | ------ | ----------- | -------- |
| text  | string |             | yes      |


## Example

This will everything given to uppercase, in this case it would return `THIS IS AN EXAMPLE`: 

```php
bot.command({
    name: "toUpperCase",
    code: `
    $toUpperCase[this is an example]
    `
});
```