## I wanted index-based string interpolation for JavaScript and was bored.

So here's **interp.js**.

And here's a [fiddle](https://jsfiddle.net/29j1v7gy/6/) to see it in action.

InterpJS appends a single function to the String object so that it supports simple index-based interpolation.

You can call `interp()` and pass parameters *like this*:

`'I wish I could write {0} {1}/{2}. :S'.interp('JavaScript', 24, 7);`

*which returns*:

`'I wish I could write JavaScript 24/7. :S'`

Or you can pass an array *like this*:

`'The {0} black {1} jumped over the other {1} {0}ly.'.interp(['quick', 'fox']);`

*which returns*:

`The quick black fox jumped over the other fox quickly.`
