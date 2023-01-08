---
title: Setup
description: Ready to begin using aoi.js, this is the basic setup you'll need to begin using aoi.js.
id: setup
---

## Installation

**node.js 16.9.0 or newer is required.**

```bash
npm install aoi.js
```

## Example

```javascript
const aoijs = require("aoi.js")

const bot = new aoijs.AoiClient({
token: "Discord Bot Token",
prefix: "Discord Bot Prefix",
intents: ["MessageContent", "Guilds", "GuildMessages"]
})

//Events
bot.onMessage()

//Command Example (ping)
bot.command({
name: "ping",
code: `Pong! $pingms`
})

//Slash Interaction Command Example (ping)
/*MUST EXECUTE FUNCTION FOR IT TO WORK
$createApplicationCommand[$guildID;ping;Pong!;true;slash]
*/
bot.interactionCommand({
  name: "ping",
  prototype: 'slash',
  code: `$interactionReply[Pong! $pingms]`
})
```