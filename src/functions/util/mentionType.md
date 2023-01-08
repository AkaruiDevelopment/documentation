---
title: $mentionType 
description: $mentionType will return the type of the mention.
id: mentionType
---

`$mentionType` will return the type of the mention.

## Usage

```php
$mentionType[mention]
```

## Parameters 


| Field   | Type   | Description         | Required |
| ------- | ------ | ------------------- | -------- |
| mention | string | any type of mention | yes      |

<details open>
  <summary> <h3> Available Types </h3></summary>

| Type     | Description                      |
| -------- | -------------------------------- |
| everyone | `@everyone` and `@here` mentions |
| users    | all user mentions                |
| roles    | all role mentions                |
| all      | everything listed above          |
 
</details>

## Example

This will return `users` as you're an user:

```javascript
bot.command({
  name: 'mentionType',
  code: `
  $mentionType[<@$authorID>]
  `
});
```
