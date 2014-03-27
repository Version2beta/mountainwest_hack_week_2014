# But really, you should learn smalltalk

Noel Rappin, @noelrap

Pharo

Smalltalk is the purist OO language

If you write scheme, you have to understand functions and recursion. Otherwise you can't use the language. Small talk is object oriented in the same way.

Smalltalk is a live dynamic environment. It's all of the system. You have access to system state in a way you can only dream of in ruby.

Smalltalk is a road not taken. An evolutionary direction in programming not followed in any significant way.

self, super, nil, true, false.

$variable
'string'
"comment"
\#symbol
\#('an', 'array')
:= assignment
^result return value
[| var | block]

Every smalltalk method has an explicit receiver

Very strict left to right control flow. 2 + 3 * 5 == 25. Can use parens to affect order of operation.

Smalltalk conditionals and block structure:

(2 > 3) ifTrue: ['Yes'] ifFalse: ['No']. "Returns false."

Loop logic is similar to Ruby

Instance variables are private and need a setter and getter.

Doesn't play well with others. Doesn't fit Unix's small programs piped together.


