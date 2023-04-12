<hr>

## Content

- Chapter 1: Start Here
- Chapter 2: Selectors
- Chapter 3: Colors
- Chapter 4: Units & Sizes
- Chapter 5: Box Model
- Chapter 6: Typography
- Chapter 7: Styling Links
- Chapter 8: List Styles 
- Chapter 9: Mini Project
- Chapter 10: Display
- Chapter 11: Floats
- Chapter 12: Columns
- Chapter 13: Position
- Chapter 14: Flexbox
- Chapter 15: Grid layout
- Chapter 16: Images
- Chapter 17: Media Queries
- Chapter 18: Card Project
- Chapter 19: Pseudo
- Chapter 20: Variables
- Chapter 21: Functions
- Chapter 22: Animations
- Chapter 23: Organization
- Chapter 24: Final Project

<hr>

## Chapter 1: Start here

- CSS, acronym for Cascade Style Sheets is a stylesheet language used to describe the presentation of a document written in HTML.

- HTML is the foundation and structure in a house example, HTML also provides **meaning** (semantics)
- CSS would be like the paint and the carpet or any decorations.
- Its all about appereance 
- CSS describes how elements should appear.

## 3 ways of applying CSS

- Inline
```html
<p style="color:#fff">This is not the way to do it!</p>
```

- External
```html
<link href="styles.css" rel="stylesheet">
```

- or Internal.

```html
<style>
	p {
		color: red;
	}
</style>
```

## Anatomy of a CSS ruleset

```css
/* selector */
p {
	color: blue;
  /* property: property value; */
	/* Declaration */
}
/* The whole structure is called a rule */
```

https://jigsaw.w3.org/css-validator/

<hr>

## Chapter 2: Selectors

- ID's should exist only once in a HTML document, they should be unique. However, it is not good practice to use id's inside your css. Typically you should use classes and sometimes element selectors, but rarely you should ever use an id selector inside your CSS. Try to keep them out of CSS. 

```css
/* Good but not enough*/
/* This is an example of that you should use a class */
p span {
	background-color: gold;
	text-transform: uppercase;
}

/* This looks way better. And you make it reusable at the same time.*/
.highlight {
	background-color: gold;
	text-transform: uppercase;
}

```