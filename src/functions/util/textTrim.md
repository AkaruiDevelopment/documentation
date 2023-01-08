---
title: $textTrim 
description: $textTrim will remove all extra spaces, multiple spaces after one space, and replaces those with one single space.
id: textTrim
---

`$textTrim` will remove all extra spaces, multiple spaces after one space, and replaces those with one single space.

## Usage

```php
$textTrim[text]
```

## Parameters 


| Field | Type   | Description            | Required |
| ----- | ------ | ---------------------- | -------- |
| text  | string | the text to be trimmed | yes      |


## Example

This will remove any extra spaces of the given text, in this case it would return `Imagine a string package.`: 

```php
bot.command({
    name: "textTrim",
    code: `
    $textTrim[Imagine          a          string package    .]
    `
});
```