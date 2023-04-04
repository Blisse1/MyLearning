
## Introduction

- Every HTML element is its own box - with its own spacing and a border. This is called the Box Model.

<hr>


- In the CSS Box Model, every HTML element is treated as a box with four areas

- Imagine you receive a box from your favorite online retailer, **the content** is the item in the box.

- The content is surrounded by a space called **padding**, similar to how bubble wrap separates an item from the box around it.

- The border is like a **cardboard box** my item was shipped in.

- **Margin** is the area outside of the box, and can be used to control the space between other boxes or elements.

```html
<!-- Even though this div has no text, its still treated as a box with content 
-->
<div></div>
```


## border behavior

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


- Esto es una prueba de manejar una branch con github