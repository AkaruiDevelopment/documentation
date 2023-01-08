---
title: $getMessage 
description: $getMessage will return properties about a given message.
id: getMessage
---

`$getMessage` will return properties about a given message.

## Usage

```php
$getMessage[channelID?;messageID?;option?]
```

## Parameters 


| Field     | Type    | Description                              | Required |
| --------- | ------- | ---------------------------------------- | -------- |
| channelID | integer | channel ID of the embed                  | yes      |
| messageID | integer | message ID of the embed                  | yes      |
| option    | string  | which part will be returned of the embed | yes      |

<details open>
  <summary><h3> Options </h3></summary>

| Type     | Description            |
| -------- | ---------------------- |
| content  | content of the message |
| userid   | author user id         |
| usertag  | author discriminator   |
| username | author username        |

</details>


## Example

This will return the content of your sent message:

```javascript
bot.command({
  name: 'getMessage',
  code: `
$getMessage[$channelID;$messageID;content]
  `
});
```