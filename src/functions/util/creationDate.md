---
title: $creationDate 
description: $creationDate will return the creation date of the given Discord User.
id: creationDate
---

`$creationDate` will return the creation date of the given Discord User.

## Usage

```php
$creationDate[id;format?]
```

## Parameters 


| Field   | Type    | Description                                         | Required |
| ------- | ------- | --------------------------------------------------- | -------- |
| id      | integer | user ID of who you want to get the creation date of | yes      |
| format? | string  | the format of the creation date                     | no       |

### Format Input

| Format        | Output                                                     |
| ------------- | ---------------------------------------------------------- |
| date          | 3/27/2018, 1:49:05 PM                                      |
| time          | 4 years, 9 months, 6 days, 2 hours, 17 minutes, 33 seconds |
| time-full     | 4 years, 9 months, 6 days, 2 hours, 17 minutes, 33 seconds |
| time-humanize | 4y 9mon 6d 2h 24m 30s                                      |


## Example

This will return your account create date:

```javascript
bot.command({
  name: 'creationDate',
  code: `
  Your account was created: $creationDate[$authorID;date]
  `
});
```
