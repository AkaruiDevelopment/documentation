---
title: $interactionPing 
description: $interactionPing will return the latency of an interaction.
id: interactionPing
---

`$interactionPing` will return the latency of an interaction.

## Usage

```php
$interactionPing
```

#### Please note that you require `bot.onInteractionCreate();` to be in your main file.

## Example

This will return the latency of an interaction:

```javascript
bot.command({
  name: 'interactionPing',
  code: `
 $addbutton[1;test;primary;testButton;no]
 Click me!
  `
});

bot.interactionCommand({
  name: 'testButton',
  prototype: 'button',
  code: `
  $interactionUpdate[This took me: $interactionPing MS!] //will edit the button message and return the latency
  `
});
```
