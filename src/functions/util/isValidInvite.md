---
title: $isValidInvite 
description: $isValidInvite will check if the given invite is valid.
id: isValidInvite
---

`$isValidInvite` will check if the given invite is valid.

## Usage

```php
$isValidInvite[url]
```

## Parameters 


| Field | Type   | Description      | Required |
| ----- | ------ | ---------------- | -------- |
| url   | string | guild invite url | yes      |


## Example

This will return `true` as `https://discord.gg/aoi-js-server-akarui-development-team-773352845738115102` is an valid invite:

```javascript
bot.command({
  name: 'isValidInvite',
  code: `
  $isValidInvite[https://discord.gg/aoi-js-server-akarui-development-team-773352845738115102]
  `
});
```
