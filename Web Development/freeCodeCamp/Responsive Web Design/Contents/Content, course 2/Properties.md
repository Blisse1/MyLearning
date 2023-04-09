<hr>

Tags: #css/properties

<hr>

## Background-image property
#css/background-image 

```css
body {
	background-image: url(#);
}
```


<hr>

## Display property
#css/display

- You can add a display property with the value inline-block so the p elements behave more like inline-elements.

```css
.item p {
	display: inline-block;
}
```

- The price didn't stay on the right. This is because inline-block elements only take up the width of their content. To spread two items out, add a width property 

<hr>

## Max-width property
#css/max-width

- The current width of the menu will always take up 80% of the body element's width. On a very wide screen, the coffee and dessert appear far apart from their prices.

- Add a max-width property to the menu class with a value of 300px to prevent it from growing too wide.

```css
.main {
	max-width: 300px;
}
```

<hr>

## Font-family property
#css/font-family

- You can change the font-family of text, to make it look different from the default font of your browser.

```css
/* This font is a fairly common one that is very readable */
body {
	font-family: sans-serif;
}
```

- It is a bit boring for all the text to have the same font-family. You can still have the majority of the text sans-serif and make just the h1 and h2 different using a different selector 

```css
h1, h2 {
	font-family: Impact;
}
```

### Fallback value

- You can make a fallback value for the font-family by adding another font name separated by a comma. Fallbacks are used in instances when the initial is not found/available.

```css
h1, h2 {
	font-family: Impact, serif;
}
```

<hr>

## Font-style property
#css/font-style

```css
/* Class selector name*/
.established {
	font-style: italic;
}
```

- The typography of heading elements (e.g h1, h2 ) is set by default valuees of user's browsers.

<hr>

## Border-color property

```css
hr {
	border-color: brown;
}
```

Notice how the thickness of the line looks bigger? The default value of a property named `border-width` is `1px` for all edges of `hr` elements. By changing the border to the same color as the background, the total height of the line is `5px` (`3px` plus the top and bottom border width of `1px`).

Change the `height` property of the `hr` to be `2px`, so the total height of it becomes `4px`

<hr>

## Background, linear-gradient 
#css/background/linear-gradient

- A gradient is when one color transitions into another. The CSS **linear-gradient** function lets you control the direction of the transition along a line, and which colors are used.

- One thing to remember is that the linear-gradient function actually creates an image element, and is usually paired with the **background** property which can accept an image as a value.

### Linear-gradient function

- It is very flexible.

```css
/* Linear gradient syntax */
linear-gradient(gradientDirection, color1, color2)
```

- gradientDirection is the direction of the line used for the transition. 
- color1, color2, are color arguments, which are the colors that will be used in the transition itself. These can be any type of color, including color keywords, hex, hsl, rgb.

- Apply a red-to-green gradient along a 90 degree line to the first marker.

```css
background: linear-gradient(90deg)
```

- The linear gradient functions needs at least two color arguments to work.
- It can accept many color arguments

```css
/* Linear-gradient function with many color arguments*/
.green {
	background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0, 255, 0), rgb(0, 0, 255));
}
```

### Color-stops

- Color stops allow you to fine-tune where colors are placed along the gradient line. They're a length unit like px or percentages that ***follow a color*** in the linear-gradient function

- For example, in this red-black gradient, the transition from red to black takes place at the 90% point along the gradient line, so red takes up most of the available space:

```css
/* Red color takes up 90% of the available space. */
/* In the same line color + color-stop */
.green {
	background: linear-gradient(90deg, red 90%, black);
}
```

- The linear-gradient function automatically calculates these values for you (*let's say you have three colors, it'll calculate so it distributes them evenly across the line* *by default*) 

- If no gradientDirection argument is provided to the linear-gradient function, it arranges colors from top to bottom, or along a 180 degree line, by default.

<hr>

## Opacity 
#css/opacity

- Opacity describes how opaque, or non-transparent, something is. For example, a solid wall is opaque, and no light can pass through. But a drinking glass is more transparent, and you can see through the glass to the other side.

- With opacity property you can control how opaque or transparent an element is. 

- With the value 0, or 0%, the element will be completely transparent, and at 1.0, or 100%, the element will be completely opaque like it is by the default.

```css
/* Opacity example. It just accept 1 value, either 0 for total transparency 
	or 1.0, so the element will be completely opaque.
*/
.sleeve {
	background-color; white;
	opacity: 0.5;
}
/* Recuerde a qué elemento le está tratando de dar opacidad, a uno especifico o uno general? */
```


<hr>


## Box-shadow css property
#css/box-shadow

- This property lets you apply one or more shadows around an element or even increment its area

```css
/* Syntax of box-shadow */
box-shadow: offsetX offsetY color;
```

- offsetX and offsetY accept number values in px and other CSS units.
- ***a positive offsetX*** value moves the shadow right and a negative value moves it left.
- ***a positive offsetY*** value moves the shadow down and a negative value moves it up.

- The height and width of the shadow is determined by the height and width of the element its applied to. You can also use an optional **spreadRadius** value to spread out the reach of the shadow

- If you want the position of your shadow on the opposite side, you can do that by using negative values for offsetX and offsetY

### Blur radius property

```css
/* Syntax of box-shadow */
box-shadow: offsetX offsetY blurRadius color;
```

- The greater value of blurRadius, the greater the blurring effect is.
- The edges of the shadow are usually sharp.

### Expanding the radius

```css
/* Syntax of box-shadow */
box-shadow: offsetX offsetY blurRadius spreadRadius color;
```

<hr>

## vertical align (property)
#css/vertical-align

- The vertical align sets vertical alignment of an inline, inline-block, or table-cell box.

- This property can be used in two contexts:
	 - To vertically align an inline element's box inside its containing line box. It could be used to vertically position an image in a line of text
	 - To vertically align the content of a cell in a table
- This only applies to inline, inline-block, and table-cell elements you cant use it to vertically align block-level elements

<hr>

## min-height property
#css/min-height

- Sets the minimum height of an element. It prevents the used value (?) of the height property from becoming smaller than the value specified for min-height.

- The element's height is set to the value of min-height whenever min-height is larger than max-height or height 

<hr>

## Overflow property
#css/overflow

- It sets the desired behavior for an element's overflow, i.e, when an element's content is too big to fit its block formatting context in both directions.
- https://developer.mozilla.org/en-US/docs/Web/CSS/overflow

- You don't always have to use pixels when sizing an element, you can do it with percentages too. And remember that percentages are relative to its parent, like in this example:

```html
<div class="frame">
	<div class="canvas">
		<div class="one"></div>
		<div class="two"></div>
		<div class="three"></div>
	</div>
</div>
```

```css
/* the width property of three class is taking 90% of the width of the parent
In this case, the parent is canvas.
*/
.three {
	width: 90%;
}
```

<hr>

## Transform property
#css/transform

- This property lets you rotate, scale, skew, or translate an element. It modifies the coordinate space of the CSS visual formatting model.

```css
.three {
	transform: rotate(0.5deg);
}
```

<hr>
