<hr>

Tags: #html/forms 

<hr>

- A web form in HTML is to *collect* information from users.
- It is make up of multiple attributes and elements.

```html
<!-- An example of a web form -->
<form action="https://freecatphotoapp.com/submit-cat-photo">
	<fieldset>
		<legend>Is your cat an indoor or outdoor cat?</legend>
		<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
		<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
	</fieldset>
	<input type="text" name="catphotourl" placeholder="cat photo URL" required>
	<button type="submit">Submit</button>
</form>
```

- If you feel unsure about any of the content of the form, you can always refer to:

	- [[Attributes]] 
	- [[Elements]]
	- [[Inputs]]

<hr>