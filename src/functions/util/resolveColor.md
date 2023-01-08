---
title: $resolveColor 
description: $resolveColor will convert a given color to a given type.
id: resolveColor
---

`$resolveColor` will convert a given color to a given type.

## Usage

```php
$resolveColor[type;returnAs?;...datas]
```

## Parameters 


| Field     | Type   | Description                               | Required |
| --------- | ------ | ----------------------------------------- | -------- |
| type      | string | which type the input is                   | yes      |
| returnAs? | string | as what the color will be returned        | no       |
| datas     | string | the data of the rgb or decimal color data | yes      |


### Types

| Types   |                   | Returns     |
| ------- | ----------------- | ----------- |
| rgb     | red, green, blue  | 50, 168, 82 |
| decimal | hex color         | #32a852     |
| number  | hexadecimal color | 80          |


## Example

This will return `#32a852` as `50, 168, 82` is the RGB value of it:

```javascript
bot.command({
  name: 'resolveColor',
  code: `
  $resolveColor[rgb;decimal;50;168;82]
  `
});
```

This will return `50, 168, 82` as `#32a852` is the hex color of it:

```javascript
bot.command({
  name: 'resolveColor',
  code: `
  $resolveColor[decimal;rgb;#32a852]
  `
});
```

This will return `3319890` as `#32a852` is the hex color of it:

```javascript
bot.command({
  name: 'resolveColor',
  code: `
  $resolveColor[decimal;number;#32a852]
  `
});
```