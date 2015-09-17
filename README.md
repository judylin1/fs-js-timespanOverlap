# Algorithm: Detect Overlapping Timespans

## Assessment

* Determine if two timespans overlap using JavaScript Date objects.

## Uses for this Algorithm

* Calendar Event Double Booking
* Meeting Scheduling
* Witness Testimony Forensics
* Library Books
* Efficient Product Shipping
* Travel Happenstance Matcher
* Gantt Chart Critical Path

## Resources

[List of Overlapping Scenarios](TimespanOverlapScenarios/README.md)

[Date Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

### Timespans

A timespan is an interval of time represented by 2 dates in time.
	Usually `start` and `end`.
The difference between the 2 dates is the total duration of the timespan.

## Exercises

### Write `isOverlapped`

Write a function, `isOverlapped` that takes in 2 timespans and determines if they overlap.

```js
function isOverlapped (timespanA, timespanB) {
	//return true if overlapping, false otherwise
}
```

For this exercise, represent timespans as objects:
```js
var christmasTimespan = {
	start: new Date("December 25, 2015"),
	end: new Date("December 26, 2015")
};
```

[Sample Data and Answers](samples/isOverlapped.js)

### Use Moment

Use [moment.js](http://momentjs.com/) instead of JavaScript Dates and repeat
	the `isOverlapped` exercise.

A timespan should be an object with Moments:
```js
var christmasTimespan = {
	start: moment("2015-12-25"),
	end: moment("2015-12-26")
};
```

Useful documentation:
* [Moment Parsing](http://momentjs.com/docs/#/parsing/)
* [Moment Queries](http://momentjs.com/docs/#/query/)

[Sample Data and Answers](samples/moment.js)

### Test Two Schedules for Overlap

Given 2 arrays of timespan objects, return any conflicting timespans between
	the 2 arrays.

```js
function scheduleOverlap(scheduleA, scheduleB) {
	// return an array of any overlapping timespans.
}
```

[Sample Data and Answers](samples/scheduleOverlap.js)
