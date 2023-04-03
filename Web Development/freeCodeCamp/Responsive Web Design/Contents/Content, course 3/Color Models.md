<hr>

Tags: #css/color-models

<hr>

## Content

 - Definition
 - rgb model
	 - CSS function
	 - Primary, secondary and tertiary colors.
 - Hex
 - HSL

<hr>

## Definition Colors 

- There are two main color models: the additive RGB (red, green, blue) model used in eletronic devices, and the subtractive CMYK (cyan, magenta, yellow, black) model used in print.

<hr> 

# rgb model
#css/rgb 

- Colors in this model begin as black and change as different levels of red, green and blue are introduced. We do this easily with the rgb function in CSS.

## rgb function

- A function is a piece of code that can take an input and perform a specific action. The CSS rgb function accepts values or *arguments* for red green and blue and produces a color

```css
rgb(red, green, blue);
```

Each red, green and blue value is a number from 0 to 255. 0 means that there is 0% of that color, and is black. 255 means that there is 100% of that color.

## Primary colors in rgb

- In additive RGB Color model, primary colors are colors that, when combined, created pure white. For this to happen, each color needs to be at its highest intensity.

```css
/* Pure red color */
.one {
	background-color: rgb(255, 0, 0);
}
```

## Secondary colors

- Are the colors you get when you combine primary colors.

```css
/* To create magenta, a combination between pure red and pure blue */
.two {
	background-color: rgb(255, 0, 255);
}
```

## Tertiary colors 

- Are created by combining a primary with a nearby secondary color.

```css
/* Tertiary color orange */
.one {
	background-color: rgb(255, 127, 0);
}
```

- To create orange, you had to increase the intensity of red and decrease the intensity of the green rgb values. This is because orange is the combination of red and yellow, and falls between the two colors in the color wheel.

![[Pasted image 20230322122719.png]]

<hr> 

## Hex values

- They're really just another form of RGB values. 
- Hex color values start with a # character and take six characters from 0-9 and A-F. The first pair of characters represent red, the second pair represent green, and the third pair represent blue.

```css
/* Green color using hex*/
.green {
	background-color: #00ff00;
}
```
- Hexadecimal or base 16 values, go from 0-9, then A-F 

0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

- With hex colors, 00 is 0% of that color, FF is 100% of that color. So '#'00ff00 translates to 0% red, 100% green, 0% blue
- Lower the intensity of that green would be like "#"007F00

<hr>

## HSL color model

- or hue, saturation and lightness, is another way to represent colors. The CSS hsl function accept 3 values: a number from 0 to 360 for hue, a percentage from 0 to 100 for saturation and a percentage from 0 to 100 for lightness

- Saturation is the *intensity* of a color from 0%, or gray, to 100% for pure color

- Lightness is how bright a color appears, from 0%, or complete black, to 100%, complete white, or 50% neutral.

<hr>
