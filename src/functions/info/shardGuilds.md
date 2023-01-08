---
title: $shardGuilds 
description: $shardGuilds will return the guilds of a specific shard.
id: shardGuilds
---

`$shardGuilds` will return the guilds of a specific shard.

## Usage

```php
$shardGuilds[option?;sep?;shardId]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| option?    | integer  | option to return the guilds in <br> 1. **id** (default) <br> 2. **name**                             | no      |
| sep?     | string  | seperator to seperate multiple guilds          | no       |
| shardId     | integer  |   the shard ID        | yes       |

#### Note that this won't work without sharding. If you're unsure, review the [sharding guide](../guides/sharding.md).

## Example

This will return the amount guilds of a shard:

```javascript
bot.command({
  name: 'shardGuilds',
  code: `
  $shardGuilds[name;, ;$shardID]
  `
});
```
