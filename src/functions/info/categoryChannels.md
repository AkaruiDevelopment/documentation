---
title: $categoryChannels 
description: $categoryChannels will return all channels of a given category.
id: categoryChannels
---

`$categoryChannels` will return all channels of a given category.

## Usage

```php
$categoryChannels[categoryID;option?;sep?]
```

## Parameters 


| Field      | Type    | Description                                                                                                                               | Required |
| ---------- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------- | :------: |
| categoryID | integer | the ID of the category                                                                                                                    |   yes    |
| option?    | string  | the option the bot will return the channels in <br> 1. **names** - returns channel names (default)  <br> 2. **ids** - returns channel IDs |    no    |
| sep?       | string  | the seperator to seperate the returned channels                                                                                           |    no    |



## Example

This will return all channels of the category of the channel where you execute the command in:

```javascript
bot.command({
  name: 'categoryChannels',
  code: `
  $categoryChannels[$channelCategoryID;names;, ]
  `
});
```