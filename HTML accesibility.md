
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