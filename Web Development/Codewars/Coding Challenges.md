## Variables challenges

### First Challenge

Given the existing code below, can you write some code so that their values are switched around?

```js
var a = "8";
var b = "3";
```

So that the variable a holds the value "8".

And the variable `b` holds the value "3".

When the code is run, it should output:

```js
 a = "3";
 b = "8";
```

### Solution

```js
var c = a;
a = b;
b = c;
```

#javascript/variables-challenges


## Strings challenges

Print the first letter of a string with mayus and the following words lower cased.

```js
var name = prompt("What is your name?"); // ANDRES, anDres, AnDrEs
var nameFormatted = name.slice(0,1).toUpperCase(); // First letter in mayus, ok
var followingWord = name.slice(1, name.length).toLowerCase(); // Following letters will always be lower cased
console.log("Welcome " + nameFormatted + followingWord); 

// I did this all by my own and the feeling it's just amazing. I just feel great to be able to do this. Sense of achivement returning back to me.
```

#javascript/strings-challenge #javascript/strings-slice-method

<hr>

What does `y`  equal?

1.  var x = 3; // 3
2.  var y = x++; // 3
3.  y += 1; // 4

## Parameters and arguments
