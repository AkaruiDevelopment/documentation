---
title: $textSplitMap 
description: $textSplitMap will create a loop over all values that are stored within $textSplit
id: textSplitMap
---

`$textSplitMap` will create a loop over all values that are stored within $textSplit.

## Usage

```php
$textSplit[awaited]
```

## Parameters 


| Field   | Type   | Description                 | Required |
| ------- | ------ | --------------------------- | -------- |
| awaited | string | name of the awaited command | yes      |


## Example

This will return the arguments within `$textSplit` and send all of them seperately: 

```php
bot.command({
    name: "textSplitMap",
    code: `
    $textSplitMap[devs]
    $textSplit[Ayaka,Leref,Ferel,Blurr;,]
    `
});

bot.awaitedCommand({
    name: "devs",
    code: `
    $message[1]
    `
});
```