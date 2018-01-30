Import rxjs

```
   var keyup = Rx.Observable.fromEvent(this.input, 'keyup')
    .map(e => {
      return e.target.value; // Project the text from the input
    })
    .filter(text => {
      return text.length > 2; // Only if the text is longer than 2 characters
    })
    // .throttleTime(500)
    .debounceTime(500)
    // .debounce(750 /* Pause for 750ms */ )
    .distinctUntilChanged()
```

Test



