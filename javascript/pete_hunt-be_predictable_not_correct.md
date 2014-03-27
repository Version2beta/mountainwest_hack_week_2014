# Be predictable not correct

Pete Hunt, @floydophone, Instagram

Good quotes on slides. Edsger Dijkstra in particular.

Simple Made Easy by Rich Hickey - good talk, look it up?

Simplicity is a lack of interleaving. (Less stuff in brain, easier to solve problem.)

"Intellectuals solve problems. Geniuses prevent them." - Albert Einstein

## Data Binding

KVO Key-Value Observation (everything but Angular, kinda)

Dirty checking (Angular)

Virtual DOM? Keep a virtual version of the DOM. Update that. Diff the real DOM. Update only what changed.

programmers believe "re-rendering and diffing is expensive"

KVO entabled app code with observables

Angular.js dirty checking forces everything through $scope, $watch, and directives

Virtual DOM needs a signal to say something has changed.

On mobile, memory is just as important as CPU

KVO bookkeeping isn't free (memory and CPU)

Virtual DOM render code is usually cheap. Few, if any, tight loops.

Views are usually smaller than models. (If not, then you probably don't have performance problems.)

"There are lies, damn lies, and Javascript performance benchmarks." - Mark Twain

Worst case scenario - needle in a haystack problem (small update, big data set)

How to solve performance problems with Virtual DOM? memoization.


