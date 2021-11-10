# Javascript essentials

## `var myVar` vs `let myVar` vs `myVar`
`var myVar`: Is function scoped
`let myVar`: Is block scoped
`myVar`: Goes to the global scope


## `use strict`

* Prevents globals.
* Without strict mode, a reference to a `this` value of null or undefined is automatically coerced to the global.

## JS common operator precedence ( Ordered by higher precedence)

[Multiplication](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators.html#Multiplication "JavaScript/Reference/Operators/Arithmetic_Operators")

left-to-right

`… * …`

[Division](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators.html#Division "JavaScript/Reference/Operators/Arithmetic_Operators")

left-to-right

`… / …`

[Remainder](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators.html#Remainder "JavaScript/Reference/Operators/Arithmetic_Operators")

left-to-right

`… % …`

13

[Addition](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators.html#Addition "JavaScript/Reference/Operators/Arithmetic_Operators")

left-to-right

`… + …`

[Subtraction](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators.html#Subtraction "JavaScript/Reference/Operators/Arithmetic_Operators")

left-to-right

`… - …`

[Equality](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators.html#Equality "JavaScript/Reference/Operators/Comparison_Operators")

left-to-right

`… == …`

[Inequality](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators.html#Inequality "JavaScript/Reference/Operators/Comparison_Operators")

left-to-right

`… != …`

[Strict Equality](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators.html#Identity "JavaScript/Reference/Operators/Comparison_Operators")

left-to-right

`… === …`

[Strict Inequality](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators.html#Nonidentity "JavaScript/Reference/Operators/Comparison_Operators")

left-to-right

`… !== …`
[Bitwise AND](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators.html#Bitwise_AND "JavaScript/Reference/Operators/Bitwise_Operators")

left-to-right

`… & …`


[Bitwise OR](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators.html#Bitwise_OR "JavaScript/Reference/Operators/Bitwise_Operators")

left-to-right

`… | …`

6

[Logical AND](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operators.html#Logical_AND "JavaScript/Reference/Operators/Logical_Operators")

left-to-right

`… && …`

5

[Logical OR](http://www-lia.deis.unibo.it/materiale/JS/developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operators.html#Logical_OR "JavaScript/Reference/Operators/Logical_Operators")

left-to-right

`… || …`

## JS functions
### reverse
_Returns_ the array in reverse order and it also reverses the order of the array _itself_.

## JS (What?)
1. 
`+ +"2"` = `2 // type number`

2. 
```
a = {}
a[{}] = 1
Object.keys(a) // ["[object Object]"]
```

## Scopes
_Arrow functions_  are more like function statements, except that they  _bind_  the  _this_  to the  _parent scope_. If the  _arrow function is in the top scope_, the  `this`  argument will refer to the  _window/global scope_, while an arrow function inside a regular function will have its this argument the same as its outer function.
