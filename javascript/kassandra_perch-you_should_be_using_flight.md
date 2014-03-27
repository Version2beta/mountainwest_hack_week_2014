# You should be using flight framework

Kassandra Perch, RetailMeNot, @kassandra_perch

Framework: essential structure

Flight:

* small set of utilities
* encourages well-written modular apps
* lightweight
* 5k gzipped, plus jquery

Not overly prescriptive

* Not MV\*
* Plays well with others
* Tools for structure, how you use it is up to you

Some characteristics

* Components are atomic
* Communication via events
* Use the DOM
* Test everything (So easy, no excuse not to)
* Heavy on functional mixins
    * Add functionality to a prototype
    * A process, not an object - Angus Croll
    * Composition over inheritance - GoF

How to:

* Write your HTML. Be semantic.
* Write your component code.
    * .defaultAttrs - assign controllers
    * .after('initialize', function() { ... });
    * Event handlers
    * require it
    * attach it

Flight component events:
* All components listening
* `this` reacts to the individual component (?)
* Error handler in .after('initialize'...)
* Stays close to the DOM with events

Testing:
* Components are atomic services
* Each service has clearly defined API
* Flight has a full testing framework (mocha-flight, jasmine-flight)
* Yeoman app generator (sets up karma and mocha-flight)
* Event spies
* Headless testing

"Testing everything would be a commandment in flight" or at least it's organized around making testing easier.

How to integrate with your existing code

* Put event handlers in your existing code
* Put event triggers in your existing code

Not intimidating.

Time to "Hello World": 15 minutes for Kassandra


