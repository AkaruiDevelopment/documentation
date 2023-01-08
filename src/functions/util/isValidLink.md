---
title: $isValidLink 
description: $isValidLink will check if the given link is valid.
id: isValidLink
---

`$isValidLink` will check if the given link is valid.

## Usage

```php
$isValidLink[url]
```

## Parameters 


| Field | Type   | Description      | Required |
| ----- | ------ | ---------------- | -------- |
| url   | string | any kind of link | yes      |


## Example

This will return `true` as the given link is valid:

```javascript
bot.command({
  name: 'isValidLink',
  code: `
  $isValidLink[https://aoi.js.org/docs/]
  `
});
```
