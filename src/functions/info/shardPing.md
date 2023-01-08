---
title: $shardPing 
description: $shardPing will return the latency of a specific shard.
id: shardPing
---

`$shardPing` will return the latency of a specific shard.

## Usage

```php
$shardPing[shardId?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| shardId?    | integer  | shard ID                             | no      |

#### Note that this won't work without sharding. If you're unsure, review the [sharding guide](../guides/sharding.md).

## Example

This will return the shard latency of the current shard:

```javascript
bot.command({
  name: 'shardPing',
  code: `
  $shardPing[$shardId]MS
  `
});
```
