---
title: $getEmbed 
description: $getEmbed will return properties about an given embed.
id: getEmbed
---

`$getEmbed` will return properties about an given embed.

## Usage

```php
$getEmbed[channelID?;messageID?;index?;option?]
```

## Parameters 


| Field     | Type    | Description                                         | Required |
| --------- | ------- | --------------------------------------------------- | -------- |
| channelID | integer | channel ID of the embed                             | yes      |
| messageID | integer | message ID of the embed                             | yes      |
| index     | integer | index of the embed, 1 first embed, 2 second embed.. | yes      |
| option    | string  | which part will be returned of the embed            | yes      |

<details>
  <summary><h3> Options </h3></summary>

| Type        | Description                     |
| ----------- | ------------------------------- |
| title       | title of the embed              |
| description | description of the embed        |
| url         | the url in the title            |
| color       | color of the embed              |
| timestamp   | timestamp located in the footer |
| fields      | field title                     |
| fvalue      | field description               |
| thumbnail   | thumbnail (image top right)     |
| image       | large image at the bottom       |
| video       | video/gif                       |
| author      | author, above title field       |
| footer      | footer                          |
| files       | attached files                  |
| createdAt   | creation date of the embed      |
| hexColor    | hex color of the embed          |
| length      | length of the embed             |

</details>


## Example

This will return the description of an embed:

```javascript
bot.command({
  name: 'getEmbed',
  code: `
$getEmbed[$channelID;messageID;1;description] //make sure to replace messageID with the actual message ID 
  `
});
```