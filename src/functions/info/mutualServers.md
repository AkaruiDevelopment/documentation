---
title: $mutualServers 
description: $mutualServers will return the mutual servers with a given user and the bot.
id: mutualServers
---

`$mutualServers` will return the mutual servers with a given user and the bot.

## Usage

```php
$mutualServers[userID?;sep?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------|----------|
| userID?      | integer  | the ID of the user                             | no      |
| sep?     | string  | the seperator to seperate the returned guilds          | no       |


## Example

This will return the mutual servers of you and the bot:

```javascript
bot.command({
  name: 'mutualServers',
  code: `
  $mutualServers[$authorID;, ]
  `
});
```
