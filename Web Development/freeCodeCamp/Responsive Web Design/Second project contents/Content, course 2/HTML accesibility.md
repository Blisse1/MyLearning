#html/accessibility

<hr>

- Make sure to use some assitive technology and screen-reader-friendly css to hide it (section) like so:

```css
.hidden {
	position:absolute;
	top: -9999px;
	left: -9998px;
}
```

https://www.tpgi.com/the-anatomy-of-visually-hidden/

"To make this decision is is helpful to put yourself in the shoes of the person using the website or the app. Once you have decided that it makes sense to hide it for everyone, you will use `display: none;` instead of the visually hidden technique."

<hr>

## Meta element description definition

- The value of the content attribute is used by search engines to provide a description of your webpage 

```html
<meta name="description" content="here you add a useful description for you web">
```

<hr>

## Navigation

- Navigation is a core part of accesibility and screen readers rely on you to provide structure of your page. This is accomplished by **semantic html elements**.

- The **header** element will be used to introduce the page, as well as provide a **navigation menu.**

- The **main** element will contain the core content of your page.

<hr>

## SVG (scalable vector graphics)

- A useful property of a svg is that it contains a **path attribute** which allows the image to be scaled **without affecting the resolution** of the resultanting image.

### Aspect-ratio property

- Sets a preferred aspect ratio for the box, which will be used in the calculation of auto sizes and some other layour functions

<hr>

## Role attribute 

 - To increase the page accessibility, the role attribute can be used to indicate the purpose behind an element on the page to assistive technologies. The role attribute is a part of the Web Accesibility Initiative (WAI) and accepts preset values. 

```html
<section role="region"></section>
```

- Every region role requires a label which helps screen readers users understand the purpose of the region. One method for adding a label is to add a heading element inside the region and then reference it with the aria-labelledby attribute. And you have to give that heading element a suitable text content.

```html

<!-- Role attribute use-->

<form method="post" action="https://freecodecamp.org/practice-project/accessibility-quiz">

	<section role="region" aria-labelledby="student-info"><h2 id="student-info">Student Info</h2></section>
	<section role="region" aria-labelledby="html-questions"><h2 id="html-questions">HTML</h2></section>
	<section role="region" aria-labelledby="css-questions"><h2 id="css-questions">CSS</h2></section>
	
</form>
```

https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/region_role

<hr>

## Typeface

- Typeface plays an important role in the accessibility of a page. Some fonts are easier to read than others, and this is specially true on low-resolution screens

<hr>

## placeholder

- Even though you added a placeholder to the first input element in the previous lesson, this is actually not best-practice for accessibility, too often, users confuse the placeholder text with an actual input value - they think is already a value in the input.
- Remove the placeholder relying on the label being the best-practice

<hr>

## sr-only attribute

- Arguably D.O.B is not descriptive enough. This is especially true for visually impaired users. One way to get around such an issue, without having to add visible text to the label, is to add text only a screen reader user can read.

- Append a span element with a class of **sr-only** to the current text content of the third label element.

```html
<div class="info">
	<label for="birth-date">D.O.B.<span class="sr-only">(Date Of Birth)</span></label>
	<input type="date" name="birth-date" id="birth-date" />
</div>

```

- The sr-only is still visible. There is a common pattern to visually hide text for only screen readers to read

```css
.sr-only{
	position: absolute;
	width: 1px;
	height: 1px;
	padding: 0;
	margin: -1px;
	overflow: hidden;
	clip: rect(0, 0, 0, 0);
	white-space: nowrap;
	border: 0;
}
```

<hr>

## Scroll-behavior property

- Clicking on the navigation links should jump the viewport to the relevant section. However, this jump can be disorienting for some users 

- Select all elements, and set the scroll-behavior to smooth

## motion-based animations (important)

- Certain types of motion-based animations can cause discomfort for some users. In particular, people with vestibular disorders have sensivity to certain motion triggers.

- The @media at-rule has a media feature called prefers-reduced-motion to set CSS based on the user's preferences. It can take one of the following values:

- reduce
- no-preference

```css
@media (feature:value){
	selectors {
		styles
	}
}

@media (prefers-reduced-motion: no-preference) {
	* {
	scroll-behavior: smooth;
	}
}

```

<hr>

## Keyboard shortcuts

- The navigation accesibility can be improved by providing keyboard shortcuts.
- The accesskey attribute accepts a space-separated list of access keys. For example:

```html
<button type="submit" accesskey="s">Submit</button>
```

- Give each of the navigation links a single-letter access key
- It is not advised to use access keys, but they can be useful.

<hr>

