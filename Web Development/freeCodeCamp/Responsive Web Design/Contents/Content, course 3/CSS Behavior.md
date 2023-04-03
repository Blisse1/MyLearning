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
