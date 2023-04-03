<hr>

Tags: #css/relative-units

<hr>

- Relative length units are relative to something else, perhaps the size of the parents element's font, or the size of the viewport. The benefit of using relative units is that with some careful planning you can make it so the size of the text or other elements scales relative to everything else on the page.

### Exploring an example

- In the example below, you can see some relative and absolute length units behave. The first box has a width in pixels. As an absolute unit, this width will remain the same no matter what else changes.

- The second box has a width set in vw (viewport width) units. This value is relative to the viewport width, and so 10vw is 10% of the width of the viewport. If you change the width of your browser window, the size of the box should change

```css
.wrapper {
	width: 10vw;
}
```

#css/vw

<hr>

### Vh (viewport height)

-  This is the same but being relative to the height of the viewport. If you shrink it from the top, it can scale doing properly.
- The vh unit stands for viewport height, and its relative to 1% of the height of the viewport

```css
.example {
	height: 10vh;
}
```

#css/vh

<hr>

### rem unit (needs completition)

- This one stands for root em, and is relative to the font size of the html element

#css/rem

<hr>