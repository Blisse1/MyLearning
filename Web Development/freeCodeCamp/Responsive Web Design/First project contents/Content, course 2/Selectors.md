<hr>

	Tags: #css/selectors

<hr>

```css
/* You can target all the p elements nested anywhere in elements with a class named item like this: */

.item p {
	property: value;
}
```

<hr>

## Type selectors with the same styling

- You can add the same group of styles to many elements by creating a list of selectors. Each selector is separated by commas like this:

```css
selector1, selector2 {
	property: value;
}
```

<hr>

## Class selector example

```css
/* To create a class, put a dot before the name */
.selector { 
	styles
}
```

<hr>

## Attribute selector 

- To style the submit button, you can use an attribute selector, which selects an element based on the given *attribute value*:

```css
/* Selecting input elements with a name attribute value of password*/
input[name="password"]{

}
```

<hr>

## Child combinator

- The child combinator > is placed between two CSS selectors. It matches only those elements matched by the second selector that are the direct children of elements matched by the first. Descendant elements further down the hierarchy don't match.

- For example to select only **p** elements that are direct children of **article**

```css
article > p 
```