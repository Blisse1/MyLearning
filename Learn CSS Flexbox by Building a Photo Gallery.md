## Intro

- Flexbox helps you design your webpage so that it looks good on any screen size.

## Box-sizing property

- If you set an element's width to 100 pixels, that 100 pixels will include any border or padding you added, and the content box will shrink to absorb that extra width. This typically makes it so much easier to size elements 

```css
/* Applying border-box to all elements. */
* {
	box-sizing: border-box;
}
```

## css behavior

- Your images are too big. Create a class to target them and give them all a width of 100% (so they can shrink) and a max-width of 350px so they shrink as needed but dont get too big. Also set the hight property to 300px to keep your images a uniform size.

```css
.gallery img {
	height: 300px;
	width: 100%; /* So they are all the same width as their parent. */
	max-width: 350px;
}
```

## Flexbox use

- Flexbox is a one-dimensional CSS layout that can control the way items are spaced out and aligned within a container.
- To use flex, give an element a display property of flex. This will make the element a **flex container**. Any direct children of a flex container are called **flex items.**

```html
<div class="container">
	<img src="#">
	<img src="#">
	<img src="#">
</div>
```

```css
/* Making the div with class container a flex container */
/* The img elements of this flex containter are called flex items*/
.container {
	display: flex;
	flex-direction: column;
}
/* You'll affect the flex-items by adding properties to the container*/
```

## Flex-direction
- The main axis is defined by **the flex-direction property**, which has four possible values:

 - row (default): horizontal axis with flex items from left to right 
 - row-reverse: horizontal axis with flex items from right to left
 - column: vertical axis with flex items from top to bottom
 - column-reverse: vertical axis with flex items from bottom to top.
 
![[Pasted image 20230409220010.png]]
- Remember to specify the flex-direction property for row value in case its the one you're using. Remember not rely on default behavior.

## Flex-wrap property.

- The flex-wrap property determines how your flex-items behave when the flex-container is too small. Remember that to affect the flex-items you must modify the flex-container.
- Setting it to **wrap** value will allow the items to wrap to the next row or column. nowrap value will prevent your items from wrapping and shrink them if needed
- Make it so your flex items wrap to the next row when they run out of space.

```css
.container {
	display:flex; 
	flex-wrap: wrap;
}

```