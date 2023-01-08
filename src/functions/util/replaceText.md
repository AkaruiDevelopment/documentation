---
title: $replaceText 
description: $replaceText will replace specific segments of text.
id: replaceText
---

`$replaceText` will replace specific segments of text.

## Usage

```php
$replaceText[text;replacer;replaceTo;times?]
```

## Parameters 


| Field     | Type   | Description                                    | Required |
| --------- | ------ | ---------------------------------------------- | -------- |
| text      | string | text you want to modify                        | yes      |
| replacer  | string | the text that will be replaced                 | yes      |
| replaceTo | string | the text that will replace `replacer`          | yes      |
| times?    | number | how many times `replaceTo` replaces `replacer` | no       |

## Examples

This will replace `M` with `D` and the output will be `Donkey`:

```javascript
bot.command({
  name: 'replaceText',
  code: `
  $replaceText[Monkey;M;D]
  `
});
```

### Advanced Examples

This will replace the word `coffee` two times using the last [field](#parameters) of `$replaceText`: 

```javascript
bot.command({
  name: 'replaceText',
  code: `
  $replaceText[I love drinking Coffee, Coffee gives me power! Coffee is bad for my health.;Coffee;orange juice;2]
  `
});
```

This will replace `Ferel` and `are` using multiple `$replaceText`:

```javascript
bot.command({
  name: 'replaceText',
  code: `
  $replaceText[$replaceText[Leref and Ferel are the same person.;Ferel;Ayaka];are;are not]
  `
});
```
