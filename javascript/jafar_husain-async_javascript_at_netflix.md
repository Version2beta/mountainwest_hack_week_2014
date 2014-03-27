# Async Javascript at Netflix

Jafar Husain, @jhusain, Netflix

Iterator and Observer patterns

Iterator pattern:

* Traverse data in a collection

* .next() or next()

Observer pattern:

* In observer pattern, producer iterates you!

What's the difference between an array and an event? Both collections!

Treat events as collections? Iterate over them?

Fat arrow lambdas in ES6

forEach, map, filter, all good

concatAll? Flatten one level. Not in JS.

LoLoMo - Netflix list of list of movies.

"Observable" - Observable === Collections + Time

* Comes from Reactive Extensions

* Can compose Events, Data requests, Animations

* see observable subscription (obj.forEach(event, error, completed)); subscription.dispose();

* Observable.forEach, .map, .filter, .concatAll

Observable of observables with concatAll?

* Oooooh - it waits for each to finish before concat'ing the next. Resolves race conditions. Sweet!

takeUntil

* Says when to stop concat'ing events

* 'this' is source collection. Arg is stop collection. {1....2}.takeUntil({...4})

switchLatest

* Cancel a pending request when a new observable starts? I think that's right. At least until last observable closes, then quit.

* Used in autocomplete in Netflix search

```
var searchResultSets = keypresses
    .throttle(50)
    .map(key => input.value)
    .filter(search => search.trim().length > 0)
    .distinctUntilChanged()
    .map(search => getJson("...").retry(3)
    .switchLatest();

searchResultSets.forEach(
    resultSet => updateSearchResults(resultSet),
    error => showMessage("The server appears to be down."));
```

Resources

* http://github.com/Reactive-Extensions/RxJS

* JavaRX - Netflix

* http://jhusain.github.io/learnrx - Netflix training on vector programming

Vector programming - helps with both concurrency and parallelism

Do this training!
