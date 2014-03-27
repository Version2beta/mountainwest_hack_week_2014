# Using TDD to tame the ball'o mud

Bandon Hayes (@tehviking)

Ball o' Mud

* Throwaway code
* Piecemeal growth
* Shantytown results

"How many of you hate to raise your hands at talks?"

"You're agile, right? So you 'agile' the code in!"

http://laputan.org/mud

Why refactor?

* Exponential change cost
* Inconsistent behavior
* Longer use = more errors

Path 1: DIY from scratch

* Make code idiomatic
* Refactor to JS objects

Path 2:

Use models

Get the hell out of the DOM

* Wrap it
* Test it
* Indentify modes
* Identify states
* Break it up

1. Wrap it with the Ember component system

* Put the code in jail - an ember component
* Move HTML to handlebar template

2. Write tests

(`Karma` for testing?)

3. Identify models

* Make a model
* Pass the unit test
* Repeat

4. Identify states

pro-tip create CSS animation and similar in state-based classes?

5. Break it up

---

No direct DOM manipulation


