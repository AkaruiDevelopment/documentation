---
title: $hasAnyPerm 
description: $hasAnyPerm will check if the user has one of the required permissions.
id: hasAnyPerm
---

`$hasAnyPerm` will check if the user has one of the required permissions.

## Usage

```php
$hasAnyPerm[guildID;userID;...perms]
```

## Parameters 


| Field   | Type    | Description                                             | Required |
| ------- | ------- | ------------------------------------------------------- | -------- |
| guildID | integer | ID of the guild where the client checks the permissions | yes      |
| userID  | integer | ID of the user                                          | no       |
| perms   | string  | permissions needed                                      | yes      |

<details>
  <summary> <h3> Discord API Permissions </h3></summary>

| Permission              |                                                                 |
| ----------------------- | --------------------------------------------------------------- |
| createinvite            | Permission to create guild invites                              |
| kick                    | Permission to kick guild members                                |
| ban                     | Permission to ban guild members                                 |
| administrator           | Administrator Permissions                                       |
| managechannel           | Permission to manage guild channels                             |
| manageguild             | Permissions to modify server settings                           |
| addreactions            | Permissions to add reactions                                    |
| viewauditlog            | Permission to view the guild's audit log                        |
| priorityspeaker         | Priority Speaker                                                |
| stream                  | Permission to stream in voice channels                          |
| viewchannel             | Permission to view a certain channel                            |
| sendmessage             | Permission to send messages in a certain channel                |
| sendtts                 | Permission to send Text-To-Speech messages                      |
| managemessages          | Permission to manage messages                                   |
| embedlinks              | Permission to embed links                                       |
| attachfiles             | Permission to attach files                                      |
| readmessagehistory      | Permission to read the message history within a certain channel |
| mentioneveryone         | Permission to mention `@everyone` and all roles                 |
| externalemojis          | Permission to use external emojis                               |
| viewguildinsights       | Permission to view guild insights                               |
| connect                 | Permission to connect to voice channels and stages              |
| mutemembers             | Permission to mute members in voice channels                    |
| deafenmembers           | Permission to deafen members in voice channels                  |
| movemembers             | Permission to move members between voice channels               |
| usevad                  | Permission to use voice-activity-detection                      |
| changenickname          | Permission to change your own nickname                          |
| managenicknames         | Permission to manage other members nicknames                    |
| manageroles             | Permission to manage roles                                      |
| managewebhooks          | Permission to manage webhooks                                   |
| manageemojisandstickers | Permission to manage emojis and stickers                        |
| useappcmds              | Permission to use application commands                          |
| requesttospeak          | Permission to use request-to-speak in stages                    |
| manageevents            | Permission to manage events                                     |
| managethreads           | Permission to manage threads                                    |
| usepublicthreads        | Permission to use public threads                                |
| useprivatethreads       | Permission to use private threads                               |
| createpublicthreads     | Permission to create public threads                             |
| createprivatethreads    | Permission to create private threads                            |
| externalstickers        | Permission to use extrernal stickers                            |
| sendmessageinthreads    | Permission to send messages in threads                          |
| startembeddedactivities | Permission to start activities within voice channels            |
| moderatemembers         | Permission to timeout and remove timeouts from guild members    |

</details>

## Example

This will return `true` when the author has `manage messages` or `kick` permissions and return `false` when they don't have any of those:

```javascript
bot.command({
  name: 'hasAnyPerm',
  code: `
  $hasAnyPerm[$guildID;$authorID;kick;managemessages]
  `
});
```

