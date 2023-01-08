---
title: Command Handlers 
description: Command Handler Setup - How to use it.
id: cmdhandler
---

## Why should you use Command Handlers?

### Storing your commands in your main file may seem fine, but after a certain amount of commands it can get hard to find and update commands. Therefore you should use the Command Handler to keep your main file neat and save yourself from the clutter.  

### Table of Content
  - [Modifying your main file][1]
  - [Creating folders and files][2]
  - [Using multiple commands in one file][3]
  - [Updating commands without restarting your Discord Bot][4]

---

### Starting off with modifying your main file

In this step we'll take a look at your main file also known as `index.js`. We add `aoijs.LoadCommands(bot)` in order for the bot to understand where our files are.

```javascript
const bot = new aoijs.AoiClient({
  token: "DISCORD BOT TOKEN",
  prefix: "DISCORD BOT PREFIX",
  intents: ["Guilds", "GuildMessages", "MessageContent"]
});

bot.onMessage(); //required for your bot to detect prefix commands

const loader = new aoijs.LoadCommands(bot)
loader.load(bot.cmd,"./commands/") //you can change this to any directory you want
```


### Setting everything up with folders and files

Once you're done with your main file, we'll move on onto files, in order for this to work we need to do two things.

1. Create directories and sub-directories where your commands go.
2. And create a file to test out if everything worked well.

#### Creating directory

Your created directory should look like that:

![commands][directory-setup-preview-1]


#### Creating sub directories

If you want to have your commands and files more organised then use sub directories, simply click on the **commands**  directory you created earlier and create as many sub directories as you want inside of it, for example, music commands:

![music][directory-sub-directory-preview-2]


#### Creating files inside of the directory

You can create as many files as you want in your directories as long as they have `.js` at the end of their file name it'll work without issues. For now, create a file called `help.js`.

![example][directory-create-file-3]

## Final Steps

### Change of creating commands

From now on you have to use:

```javascript
module.exports = [{...}]
```

Open your `help.js` and copy & paste the following code snippet: 

```javascript
module.exports = [{
  name: "help",
  aliases: ["helpcmd", "helpme"],
  code: `
$title[Help Command!]
$thumbnail[$authorAvatar] 
$description[Any text you like can go here!]
$footer[Even footers!]`
}];
```

Now restart your bot, and let the magic happen! Simply use `[prefix]help` or any of the aliases to make the message appear.

### Multiple commands in one file

From now on, you can have multiple commands in one file, this is useful for `awaited` commands or any similar. Let's create a little nice welcome command and combine the command from above with it! 

```javascript
module.exports = [{
  name: "help",
  aliases: ["helpcmd", "helpme"],
  code: `
$title[Help Command!]
$thumbnail[$authorAvatar] 
$description[Any text you like can go here!]
$footer[Even footers!]`
}, {
  type: "join",
  channel: "any channel ID",
  code: `
$title[Someone joined!!]
$description[Welcome to this server <@$authorID>!]`
}]
```

> ⚠ Make sure you have the required intents and `bot.onJoin();` in your `index.js` or else this won't work!
>
> Required intents: `guildMembers`

### Updating your commands without restart!

You are able to use `$updateCommands` when updating commands in your directory. Please note that this does **not** apply to any files outside of the directory.


<!--- links -->
[1]: #starting-off-with-modifying-your-main-file
[2]: #setting-everything-up-with-folders-and-files
[3]: #final-steps
[4]: #updating-your-commands-without-restart
[directory-setup-preview-1]: https://cdn.discordapp.com/attachments/901271834589278228/1059592951304556664/image.png
[directory-sub-directory-preview-2]: https://cdn.discordapp.com/attachments/901271834589278228/1059592950998368336/image_1.png
[directory-create-file-3]: https://cdn.discordapp.com/attachments/901271834589278228/1059598511278137455/image_2.png
