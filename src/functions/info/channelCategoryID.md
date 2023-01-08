---
title: $channelCategoryID 
description: $channelCategoryID will return the parent of a specific channel.
id: channelCategoryID
---

`$channelCategoryID` will return the parent of a specific channel.

## Usage

```php
$channelCategoryID[channelID?]
```

## Parameters 


| Field      | Type    | Description                                                         | Required |
| ---------- | ------- | ------------------------------------------------------------------- | :------: |
| channelID? | integer | channel ID of a channel of which you want to retrieve its parent of |    no    |


## Example

This will return the category ID of the text channel in where you execute the command:

```javascript
bot.command({
  name: 'channelCategoryID',
  code: `
  $channelCategoryID[$channelID]
  `
});
```