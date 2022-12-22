---

description: Initial description.

author: "@Luigi"
---

title:: Temporal.js

- ```
  Temporal.Now.plainDateTimeISO()
  ```
	- this is for moment() to refer to now
- const now = Temporal.Now.plainDateISO().toString() 2022-06-15
- const now = Temporal.Now.zoneDateTimeISO().toString() adds timezone
- Methods
	- Temporal.Duration
	- Temporal.Instant
	- Temporal.Now
-
	- Temporal.PlainDate
		- Temporal.PlainDate(2022,06,15)
		- Temporal.PlainDate.from("2022-06-15") // creates date from string
		- Temporal.PlainDate.from({ year:2022, month:6, day:15})
	- Temporal.PlainMonthDay
	- Temporal.PlainTime
	- Temporal.Now.timeZone()  retrieves the current time zone
	-
	-
	-
	-
- const now = Temporal.Instant.from("string")
-
- ADDING DAYS, ETC
	- Temporal.Now.plainDateISO().add({days:1})
		- also subtract