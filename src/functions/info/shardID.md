---
title: $shardID 
description: $shardID will return the current shard ID.
id: shardID
---

`$roleCount` will return the current shard ID.

## Usage

```php
$shardID
```

#### Note that this won't work without sharding. If you're unsure, review the [sharding guide](../guides/sharding.md).

## Example

This will return the current shard ID:

```javascript
bot.command({
  name: 'shardID',
  code: `
  I'm currently on shard $shardID!
  `
});
```
