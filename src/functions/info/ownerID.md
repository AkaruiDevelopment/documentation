---
title: $ownerID 
description: $ownerID will return the ID of the server owner, depending on the given argument.
id: ownerID
---

`$ownerID` +will return the ID of the server owner, depending on the given argument.

## Usage

```php
$ownerID[guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------|----------|
| guildID?     | integer  | guild ID          | no       |


## Example

This will return the ID of the server owner where you execute the command in:

```javascript
bot.command({
  name: 'ownerID',
  code: `
  $ownerID[$guildID]
  `
});
```
