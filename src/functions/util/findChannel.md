---
title: $findChannel 
description: $findChannel will search a given channel by its name.
id: findChannel
---

`$findChannel` will search a given channel by its name.

## Usage

```php
$findChannel[channel;returnSelf?]
```
#### Note that your bot has to be present in the guild where the channel is in.
## Parameters 


| Field       | Type   | Description                                                                                            | Required |
| ----------- | ------ | ------------------------------------------------------------------------------------------------------ | -------- |
| channel     | string | channel name of the channel you want to find                                                           | yes      |
| returnSelf? | string | will return the channel where the command is executed in by default if the given channel was not found | no       |


## Example

This will return `882360051640193054` as it was able to find the `#⊂・⊃﹐aoi_v5` channel:

```javascript
bot.command({
  name: 'findChannel',
  code: `
  $findChannel[⊂・⊃﹐aoi_v5;no]
  `
});
```
