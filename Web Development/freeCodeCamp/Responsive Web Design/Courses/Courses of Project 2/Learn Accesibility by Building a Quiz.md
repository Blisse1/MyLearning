<hr>

## Content

- New meta element learned
- Navigation
- SVG
	- Aspect-ratio property
- Role attribute
- Typeface
- sr-only class
- New pseudo-element learned, ::before
- Default styling list-items
- Scroll-behavior property
- Placeholder use
- CSS behavior, lists on small screens
	- Remove style of a list.
- Motion-based animations
- Keyboard shortcuts
- Additional Notes and Assistive Tips


<hr>

## Additional Notes

- The lang attribute on the html will assist screen readers in identifying the language of the page
- Meta element is used to specify information about the page, such as title, description, keywords and author 
- On topic of visual accessibility, contrast between elements is a key factor. For example, the contrast between the text and the background of a heading should be at least 4:5:1

<hr>

## Navigation to headings with href

- To be able to navigate within the page, give each anchor element an href corresponding the id of the h2 elements

```html
<ul>
	<li><a href="#student-info">INFO</a></li>
	<li><a href="#html-questions">HTML</a></li>
	<li><a href="#css-questions">CSS</a></li>
</ul>
```

<hr>

## Assistive tips

- It is important to link each input to the corresponding label element. This provides assistive technology users with a visual reference to the input.
- This is done by giving the label a for attribute, which contains the id of the input.

```html
<section role="region" aria-labelledby="student-info">

	<h2 id="student-info">Student Info</h2>
	<div class="info">
		<label for="student-name">Name: </label>
		<input id="student-name"/>
	</div>
	<div class="info">
		<label for="email">Email: </label>
		<input id="email"/>
	</div>
	<div class="info">
		<label for="date-of-birth">Birth: </label>
		<input id="date-of-birth"/>
	</div>

</section>

```

<hr>






