get the allergy record of a user.

`getAllergyRecord` accepts an options object containing optional *`date: ISO8601Timestamp`*. if `date` is not provided it will default to the current time.
```javascript
let options = {
    date: (new Date(2016,5,1)).toISOString(), // optional; default now
};
```

```javascript

AppleHealthKit.getAllergyRecord(options: Object, (err: Object, results: Object) => {
  if (err) {
    return;
  }
  console.log(results);
});
```

```javascript
{
	startDate: '2016-07-08T12:00:00.000-0400',
	endDate: '2016-07-08T12:00:00.000-0400'
}
```