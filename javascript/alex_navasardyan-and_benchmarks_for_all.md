# And benchmarks for all!

Alex Navasardyan, @twokul

http://bit.ly/1fgDo2g

Your javascript -> Compiler -> Native code

Optimizations of the compiler may result in different results than you think you're benchmarking.

What you need to know to write benchmarks: A little bit about compilers

* Hidden classes - JS is dynamically typed, prototype-based language. New classes (are? may be?) created when the shape of a class changes, for instance when adding a new property to one instance.
* Inline cache - Don't run the function if compiler can cache it, I think.

How to benchmark

* Iterations - rather than a set number of times through the code, try running for at least X seconds.
* jsPerf.com - precise timers and better patterns.

Takeaway seems to be jsPerf.com - precise timers and better patterns.

* benchmarkjs.com?
* IRHydra?

