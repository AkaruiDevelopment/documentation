---
title: $formatDate 
description: $formatDate will format a given date.
id: formatDate
---

`$formatDate` will format a given date.

## Usage

```php
$formatDate[date;format?]
```

## Parameters 


| Field   | Type   | Description                                      | Required |
| ------- | ------ | ------------------------------------------------ | -------- |
| date    | number | the date you want to format                      | yes      |
| format? | string | the format that will be used to display the date | no       |


<details open>
  <summary> <h2> Possible formatting </h2></summary>

| Format |                                                            |
| ------ | ---------------------------------------------------------- |
| dddd   | Returns the weekday, Monday, Tuesday, Wednesday ...        |
| dd     | Returns the abbreviation of the weekday, Mon, Tue, Wed ... |
| DD     | Returns the day of the month                               |
| DDD    | Returns the day of the year, 256, 257 ...                  |
| MMMM   | Returns the month fully January, February ...              |
| MMM    | Returns the abbreviation of the month, Jan, Feb ...        |
| MM     | Returns the month of the year, 10, 11 ...                  |
| YYYY   | Returns year fully, 2020, 2021 ...                         |
| YY     | Returns the last two numbers of the year, 20, 21 ...       |

</details>

## Example

This will return your current date in the `dddd, DD MMMM YYYY` format:

```javascript
bot.command({
  name: 'formatDate',
  code: `
  $formatDate[$dateStamp;dddd, DD MMMM YYYY]
  `
});
```
