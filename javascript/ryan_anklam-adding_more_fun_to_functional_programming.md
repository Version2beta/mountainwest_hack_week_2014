# Adding Even More Fun to Functional Programming With RXJS

Ryan Anklam, @bittersweetryan, Netflix

Functional review with Rx twists

* Map - data transformation

* Filter - narrows collections

* Reduce - turn a collection into a single value

Reduce a collection into a unorderd list??

* Zip - Combine collections with a function

Wow, observables are pretty damn cool

throttle(...).filter(...).map(...).distinctUntilChanged(...).reduce(...)

doesn't run until observable.forEach (?!)

Think functionally

* Replace loops with map, reduce, filter

* Replace if's with filters

* Don't put too much in a single stream. Smaller streams are okay.

Streams are filters on observables too.

Flattening patterns

* Manages concurrency in observables

* Observables = events over time

* Three flattening patterns

    * merge - combine items in a collection as each item arrives

    * concat - combine collections in the order they arrive

    * switchLatest - switch to the latest collection that arrives, ignoring the rest of previous collections

DOM manipulation only in forEach, not in maps, reduces, filters, zips, concats, etc.


