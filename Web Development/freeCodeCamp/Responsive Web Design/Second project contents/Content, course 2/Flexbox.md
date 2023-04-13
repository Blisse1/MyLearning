<hr>

## Content

- Definition / use
- Properties
	- Flex-direction
	- Flex-wrap
	- Justify-content
	- Align-items
- Notes

<hr>

## Flexbox use
#css/flexbox

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

<hr>


## Flex-direction
#css/flexbox/flex-direction

- The main axis is defined by **the flex-direction property**, which has four possible values:

 - row (default): horizontal axis with flex items from left to right 
 - row-reverse: horizontal axis with flex items from right to left
 - column: vertical axis with flex items from top to bottom
 - column-reverse: vertical axis with flex items from bottom to top.
 
![[Pasted image 20230409220010.png]]
- Remember to specify the flex-direction property for row value in case its the one you're using. Remember not rely on default behavior.

<hr>

## Flex-wrap property.
#css/flexbox/flex-wrap 

- The flex-wrap property determines how your flex-items behave when the flex-container is too small. Remember that to affect the flex-items you must modify the flex-container.
- Setting it to **wrap** value will allow the items to wrap to the next row or column. nowrap value will prevent your items from wrapping and shrink them if needed
- Make it so your flex items wrap to the next row when they run out of space.

```css
.container {
	display:flex; 
	flex-wrap: wrap;
}
```

<hr>


## Justify-content property (main axis)
#css/flexbox/justify-content

- It determines how the items inside a **flex container** are positioned along **the main axis** (the horizontal one), affecting their position and the space around them.

### Space-between property
- Items are evenly distributed in the line; first item is on the start line, last item is on the end line. 

<hr>


## Align-items property (cross axis)
#css/flexbox/align-items

- It positions the flex content along the **cross axis**. In this case, with your flex-direction set to row, your **cross axis** would be vertical.
- To vertically center your images, give your .gallery selector an align-items property with center as the value

![[Pasted image 20230410070633.png]]

- With the max-width property you can allow the items to expand to certain width.

<hr>

## flexbox tip
#css/flexbox-tip

- El contenido de un elemento también cuenta como *contenido* de flex

```html
<p class="ejemplo">Texto afectado</p>
```

```css
/*Justify-content property will affect the content of the p element
in this case it would be Texto afectado
*/
.ejemplo {
	display: flex;
	justify-content: flex-end;
}
```

<hr>
