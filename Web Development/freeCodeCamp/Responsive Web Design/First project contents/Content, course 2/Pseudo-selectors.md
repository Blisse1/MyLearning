<hr>

Tags: #css/pseudo-selectors

<hr>

- You can change properties of a link when the link has actually been visited by using a pseudo-selector that looks like:

```css

a:visited {
	color: grey;
}

```

- You can change the properties of a link when the mouse hovers over them by using the pseudo-selector that looks like:

```css
a:hover {
	color: green;
}
```

- You can change the properties of a link when the link is actually being clicked by using a pseudo-selector that looks like: 

```css

a:active {
	color: blue;
}

```

- The menu text `CAMPER CAFE` has a different space from the top than the address's space at the bottom of the menu. This is due to the browser having some default top margin for the `h1` element

<hr>

## CSS pseudoclass

- You can select the last element of a specific type using last-of-type css pseudo class:

```css
/* Last p */
p:last-of-type {

}
```

<hr>
