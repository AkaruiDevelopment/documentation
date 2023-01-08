---
title: $cpu 
description: $cpu will return CPU usage of a process or the OS.
id: cpu
---

`$cpu` will return CPU usage of a process or the OS.


## Usage

```php
$cpu[option?]
```

## Parameters 


| Field   | Type   | Description                                                                                                                                                      | Required |
| ------- | ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------: |
| option? | string | the option that the cpu usage will be returned of <br> 1. **os** - returns the CPU usage of the bot <br> 2. **process** - returns the CPU usage of the process |    no    |


## Example

This will return the CPU usage of your bot:

```javascript
bot.command({
  name: 'cpu',
  code: `
  OS: $cpu[os] 
  Process: $cpu[process] // around %0 
  `
});
```