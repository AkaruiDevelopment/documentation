---
title: $toLowerCase 
description: $toLowerCase will change the given text from uppercase to lowercase.
id: toLowerCase
---

`$toLowerCase` will change the given text from uppercase to lowercase.

## Usage

```php
$toLowerCase[text]
```

## Parameters 


| Field | Type   | Description | Required |
| ----- | ------ | ----------- | -------- |
| text  | string |             | yes      |


## Example

This will everything given to lowercase, in this case it would return `aoi.js is great.`: 

```php
bot.command({
    name: "toLowerCase",
    code: `
    $toLowerCase[AOI.JS IS GREAT.]
    `
});
```