#css/behavior

<hr>

## Div behavior

```html
<!-- Two divs next to each other, stack like actual blocks -->
<div class="marker red">
	<div class="cap"></div>
	<div class="sleeve"></div>
</div>
```

```css
.marker {
width: 200px;
height: 25px;
margin: 10px auto;
}
.cap {
width: 60px;
height: 25px;
}
.sleeve {
width: 110px;
height: 25px;
background-color: rgba(255, 255, 255, 0.5);
}
```

- Your new cap div is taking up the entire width of the marker, and is pushing the sleeve down to the next line.

- This is because the default display property for div elements is ***block***. So when ***two block elements*** are next to each other, **they stack like actual blocks**. Sin importar qué tanto width tengan el uno del otro.

- To position two div elements on the same line, set their display properties to inline-block.

### To solve it

- Target both classes and add display's property value to inline-block.

```css
.sleeve, .cap {
	display: inline-block;
}
```


<hr>

```html
<!-- Body element being the parent of the div -->
<body>
	<div>
		<main>
			<h1>CAMPER CAFE</h1>
			<p>Est. 2020</p>
			<section>
			<h2>Coffee</h2>
			</section>
		</main>
	</div>
</body>
```

```css
/* We're making here the div to be the 80% of the width of its parent element*/
/* Remember that the parent element of this div is the body element*/
/* Basically the one where the div is contained.*/
div {
	width: 80%;
}
```

<hr>

## Centering a div horizontally

- You can do this by setting its margin-left and margin-right properties to auto.

<hr>

## Same line of the editor to make it evenly spaced.

```html
<p class="flavor">French Vanilla</p><p class="price">3.00</p>
```

```css
.flavor, .price {
	width: 50%;
}
```

<hr>

## Behavior CSS

- Fix its size to a maximum width of 500px, a min-width of 300px. In between that range, allow it to have a width of 60vw

<hr>

## Curiosidad (behavior)

- Se le puede cambiar el background a un input, por ejemplo en este caso se le está colocando un fondo de cierto color para que haga contraste con el fondo de la página

<hr>

## width unset css value

- This will remove an earlier rule if any which may have setted all the input elements to certain width

```css

.inline {
	width: unset;
}

```

<hr>

## border and padding behavior

```html
<div class="frame">
	<div class="canvas"></div>
</div>
```

```css
.frame {
	border: 50px solid black;
}
```

- Si tenemos esto de esta manera, y le aplicamos luego un border al frame, significa que aplicará el borde hacia dentro y no hacia afuera, a como está usted acostumbrado a verlo.

- Funciona como un padding cuando se tiene un elemento dentro de otro.

```css
.frame {
	border: 50px solid black;
	padding: 50px;
}
/* Lo que hace este padding es ampliar el espacio que hay entre .frame
y el elemento que contiene, en este caso .canvas.
*/
```

- You use the margins to adjust the spacing outside of an element.

- Now .one is centered horizontally, but its top margin is pushing past the canvas and onto the frame's border, shifting the entire canvas down 20 pixels.

![[Pasted image 20230404085853.png]]

```html
<div class="frame">
	<div class="canvas">
		<div class="one"></div>
	</div>
</div>
```

```css
.canvas {
	padding: 1px;
}
```


- Add padding of 1px to the .canvas element to give the .one element something solid to push off of.

![[Pasted image 20230404090028.png]]

- Adding 1 px of padding to the top, bottom, left and right of the canvas changed its dimensions to  502 pixels x 602 pixels

- Replace the padding property with **overflow set to hidden**, changing the canvas back to its original dimensions

<hr>

## CSS behavior (images)

- Your images are too big. Create a class to target them and give them all a width of 100% (so they can shrink) and a max-width of 350px so they shrink as needed but dont get too big. Also set the hight property to 300px to keep your images a uniform size.

```css
.gallery img {
	height: 300px;
	width: 100%; /* So they are all the same width as their parent. */
	max-width: 350px;
}
```

<hr>

## Distorted images, object-fit property
#css/object-fit

- Notice how some of your images have become distorted. This is because the images have different aspect ratios. Rather than setting each aspect ratio individually, you can use the object-fit property to determine how images should behave.

- Give your .gallery img selectr the object-fit property and set it to **cover** value. This will tell the image to fill the img container while maintaining aspect ratio, resulting in cropping to fit.

<hr> 

## space between flex-items 
#css/gap

- The **gap** CSS shorthand property sets the gaps, also knowns as gutters, between **rows and columns** The gap property and it's row-gap and column gap sub-properties provide this functionality for flex, grid, and multi-column layout. You apply the property to the container element.

```css
/* Applied to the container */

.container {
	gap: 16px;
}
```