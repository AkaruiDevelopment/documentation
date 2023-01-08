---
title: $uptime 
description: $uptime will return the bot's uptime.
id: uptime
---

`$uptime` will return the bot's uptime.

## Usage

```php
$uptime[option?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------| :------: |
| option?    | string  | how the uptime will be returned | no      |

| Option     | Output    | 
|-----------|---------|
| full **(default)**  | 19 minutes, 21 seconds  |
| humanize   | 19m 21s  |
| ms   | 1165980  |

## Example

This will return the time of how long your bot is online for:

```javascript
bot.command({
  name: 'uptime',
  code: `
  I've been up for $uptime[full]!
  `
});
```
