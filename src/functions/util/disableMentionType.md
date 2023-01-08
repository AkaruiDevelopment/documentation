---
title: $disableMentionType 
description: $disableMentionType will disable a specific mention type.
id: disableMentionType
---

`$disableMentionType` will disable a specific mention type.

## Usage

```php
$disableMentionType[type]
```

## Parameters 


| Field | Type   | Description                         | Required |
| ----- | ------ | ----------------------------------- | -------- |
| type  | string | type of mention you want to disable | yes      |


<details>
  <summary> <h2> Available Types </h2></summary>

| Type     | Description                      |
| -------- | -------------------------------- |
| everyone | `@everyone` and `@here` mentions |
| users    | all user mentions                |
| roles    | all role mentions                |
| all      | everything listed above          |
 
</details>

## Example(s)

This will stop the bot from mentioning you:

```javascript
bot.command({
  name: 'mention',
  code: `
<@$authorID>
$disableMentionType[users] 
  `
});
```

This will stop the bot from mentioning anyone or anything:

```javascript
bot.command({
  name: 'mention',
  code: `
<@$authorID>
$disableMentionType[all] 
  `
});
```
