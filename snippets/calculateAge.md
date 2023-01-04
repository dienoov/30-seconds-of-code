---
title: Calculate age
tags: date
firstSeen: 2023-01-04T03:59:21+00:00
---

Calculate age from given date.

- Use the `Date` constructor to get the current date and to create a date from the given date.
- Subtract the current date from the given date, then divide it by 1000 (milliseconds), 60 (seconds), 60 (minutes), 24 (hours), and 365.25 (days).
- Use the `Math.floor()` method to round the calculated age down to the nearest integer.

```js
const calculateAge = date =>
  Math.floor((new Date() - new Date(date)) / 1000 / 60 / 60 / 24 / 365.25);
```

```js
calculateAge('03/20/2003'); // 19
```
