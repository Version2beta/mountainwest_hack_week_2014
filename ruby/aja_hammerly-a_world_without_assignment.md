# A world without assignment

Aja Hammerly, Substantial.com, @thagomizer_rb

## Functional programming

"The entire idea of mutable state is suspicious and easy to mess up."

## Focus, no assignment

* 114 slides
* Lots of code
* No assignment

## Scheme

* From Lisp, sibling to CLisp
* Prefix notation
* Function definitions are easy
* `cond`
* `#t` true, `#f` false
* List `'(1 2 3)`
* `car` head of list 1
* `cdr` tail of list (2 3)
* Empty list `(null? '())` - #t
* Recursion
    * Factorial
    * Fibonacci
    * Exponentiation

```
(define (expt b n)
  (expt-t b n 1))
(define (expt-t b c p)
  (if (= c 0)
    p
    ...
```

## Example problem, change from a dollar

How many ways can you make change for a dollar using quarters, dimes, nickels, and pennies?

In functional programming `case` statements are awesome.

```
def cc(amount, coins)
    case
    when coins.empty?
        0
    when amount < coins.first
        cc(amount, coins.rest)
    when amount == coins.first
        1 + cc(amount, coins.rest)
    else
        cc(amount, coins.rest) + cc(amount - coins.first, coins)
    end
end
```

Assumes coins is alist of coins in descending order.

## Other functions

* Member
* Any
* Lambda

## Learning more

* The Little Schemer, book, Socratic dialog. Weird. Good.
* The Seasoned Schemer
* The Reasoned Schemer
* Structure and Interpretation of Commputer Programmers
