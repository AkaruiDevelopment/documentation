---
title: $replaceTextWithRegex
description: $replaceTextWithRegex will replace specific regex in a text. This works similar as $replaceText.
id: replaceTextWithRegex
---

`$replaceTextWithRegex` will replace specific segments of text.

## Usage

```php
$replaceTextWithRegex[text;reg;flags;newT]
```

## Parameters 


| Field | Type   | Description                      | Required |
| ----- | ------ | -------------------------------- | -------- |
| text  | string | text you want to modify          | yes      |
| reg   | string | the regex that will be replaced  | yes      |
| flags | string | [flags](#flags)                  | yes      |
| newT  | string | the text that will replace `reg` | no       |

<details open>
  <summary><h2> Flags </h2></summary>

| Flags |                                        |
| ----- | -------------------------------------- |
| g     | Replace all matches (case-sensitive)   |
| m     | Multiline matching                     |
| i     | Replace all matches (case-insensitive) |

</details>

## Examples

This will replace `more` with `less`:

```javascript
bot.command({
  name: 'replaceTextWithRegex',
  code: `
  $replaceTextWithRegex[This function is more complicated than it looks.;more;g;less]
  `
});  
```

### Advanced Example
 
This will replace `more` with `less`:

```javascript
bot.command({
  name: 'replaceTextWithRegex',
  code: `
  $replaceTextWithRegex[This function is more complicated than it looks.;lESs;i;more]
  `
});  
```