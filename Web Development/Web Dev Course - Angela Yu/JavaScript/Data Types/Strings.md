## Strings

A string is a way of classifying data to tell the computer how the program intends to use the data. It's a string of characters.

```js
alert("Hello");
```

#javascript/strings

## Concatenation

```js
alert("a" + " " + "b");

// a b
```

## How to get the number of characters out of a string

```js
var name = "Andres";
name.length;

// 6 as result
```

## Slice method

```js
var name = "Angela";
name.slice(0, 6); // Angela
name.slice(1, 5); // ngela
name.slice(5, 0); // a
```

## toUpperCase method

It changes all the characters of a string to upperCase.