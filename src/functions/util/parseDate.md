---
title: $parseDate 
description: $parseDate will return the date/time for the given milliseconds
id: parseDate
---

`$parseDate` $parseDate will return the date/time for the given milliseconds

## Usage

```php
$parseDate[ms;type?]
```

## Parameters 


| Field | Type   | Description                                           | Required |
| ----- | ------ | ----------------------------------------------------- | -------- |
| ms    | string | time in ms you want to parse                          | yes      |
| type? | string | the type in which the parsed date will be returned in | no       |

### Types
| Type | Format                                                   |
| ---- | -------------------------------------------------------- |
| time | 1 years, 1 week, 6 days, 8 hours, 16 minutes, 20 seconds |
| date | 1/1/2023, 8:16:20 AM                                     |


## Example

This will return your current date in the `date` [format](#types):

```javascript
bot.command({
  name: 'parseDate',
  code: `
  $parseDate[$dateStamp;date]
  `
});
```
