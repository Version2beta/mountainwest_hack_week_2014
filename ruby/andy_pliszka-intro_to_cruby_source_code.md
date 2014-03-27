# Introduction to CRuby Source Code

Andy Pliszka, Pivotal Labs, @antityping

Understanding Ruby

* Object Model
* Metaprogramming
* Garbage Collection

Speed up Ruby

* Rewrite parts in C
* 10x - 50x faster - profit!

C Extensions

Ruby + C

* Ruby ecosystem
* C Speed, efficiencies

Level 1: Build Ruby from scratch (30 minutes)

* uses autoconf
* requires openssl
* set paths
* verify with `gem env` too
* `gem install rails --no-docs` is good too

Level 2: Debuggin

Debuggers: varied. `gbd`, `xcode`, `lldb`, etc.

Level 3: Ruby classes and methods in C

Method definition in C

* `rb_define_method(cb_cArray, "length", rb_Ary_length, 0)`

Class definition

* `rb_define_class`
* `rb_define_alloc_function`
* ...

C

* memory management
* malloc/free

Ruby

* garbage collection

Level 4: Converting Ruby to C

fibanacci example in presentation about 30x faster

Level 4b: Change '+' to '-' for the delight of your coworkers.

Level 5: Graphs

Andy skipped quickly through this

Is it safe in production? Nope, not unless you're good at it :-)

Epilog

* Ruby internals
* Ruby metaprogramming
* Ruby object model
* Use C for moar speed
* Easy to rewrite hot functions in C
* Original C algorithm code can be used without modification

