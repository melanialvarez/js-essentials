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
3.
`true == 1 // true`
`false == 0 // true`

4.
```
typeof NULL // "undefined"
typeof null // "object"
```
## Scopes
_Arrow functions_  are more like function statements, except that they  _bind_  the  _this_  to the  _parent scope_. If the  _arrow function is in the top scope_, the  `this`  argument will refer to the  _window/global scope_, while an arrow function inside a regular function will have its this argument the same as its outer function.

## Hoisting
JS has two stages
* compilation
	* Variables `var` are created in memory (without the value, so they will be assigned the value undefined)
	* Variables `let, const` are created in memory (without any assignment so if you try to access them before the line where they are assigned to a value, it throws an error).
	* Functions are also created in memory.
* execution

# CSS
## box model
`box-sizing: content-box;` // Default (border takes pixels)
`box-sizing: border-box;` // the width will set the max value the element can have (including border)

## display
`block` will take all available width

`inline` will take as less space as possible (fit the content)

`inline-block` will take as less space as possible (fit the content) but you can set width and height to the element.

`none` will hide element

### flexbox
(*) most important attributes needed to create complex flex containers.
#### container:
```
display: flex
flex-direction: row
				column
*justify-content: flex-start
				 center
				 space-between // items don't have space to the container edges. (width)
				 space-around // gives a margin to the container's edges. (width)

*align-items: // how is the height of elements going to be treated.
			 stretch // will stretch all items to tallest height 
			 flex-start // will keep original height of element
			 center // will center vertically :O

flex-wrap: wrap // when screen size goes smaller, items will break to new line

align-content: // align content vertically (top, bottom)
				center
				flex-start //top
				flex-end // bottom
				space-between // same as above but for vertical space
```

#### items 
```
*flex-shrink: 0 // don't change width of item when resizing (keep width defined in elment always)
*flex-grow: 1 // it can have 1,2... any number to indicate how grow will work compared to other elements, if el1 has grow:1, and el2 has grow:2, then el2 will have (approximately) the double of the width of el1. I say approximately because if el1 had an predefined width, that would be taken as starting point.
flex-basis: 0 // defines the starting point (weight). So it will allow that el2 is actually twice as el1.
align-self: center // like align-items property but set to only one element
order: <any number> // set order of element
```


## media queries

`all`

Suitable for all devices. It can be omitted and it will work

`print`

Intended for paged material and documents viewed on a screen in print preview mode.

`screen`

Intended primarily for screens.

`speech`

Intended for speech synthesizers. (screen readers)

```
@media all and (max-width="300px") // from 0 to 300px it will take this style
	...
```


```
@media all and (min-width="300px") // from 300px to screen width size it will take this style
	...
```

