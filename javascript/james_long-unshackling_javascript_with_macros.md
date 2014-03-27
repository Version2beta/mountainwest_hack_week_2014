# Unshackling Javascript with Macros

James Long, @jlongster, Mozilla, sweet.js

Stop Writing Javascript Compilers! Make Macros Instead - blog post by James Long. Definitely read.

# Macros

Without macros: parse - compile - execute

With macros: expand - parse - compile - execute

(Note to self: How to read code would be an interesting talk.)

Pattern matching macros

`let` macros

* let macros are recursive

Repeating patterns

Case macros

http://jlongster.com/Writing-Your-First-Sweet.js-Macro

Jame's rules for writing macros:

* Don't write a macro

* Don't break JS syntax

* Macros as expressions invoked with parens

* Macros as statements invoked with braces

Clojure core.async?

Some macros

* ES6 macros

* Static allocation

* Pattern matching

Not implemented yet:

* Generators

* React.js syntax natively
