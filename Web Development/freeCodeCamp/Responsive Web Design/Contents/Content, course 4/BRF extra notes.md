## How do you get rid of the horizontal scroll-bar in CSS?

- You can set margin to 0, since it has some default settings.

- Color en el body representa color del texto en todo el documento

<hr>

## Do not forget the accesibility best practices!

- If you have a form with inputs and labels, do not forget to link them using a for attribute!

```html
<!-- Inputs and labels linked-->
<fieldset>
	<label for="first-name">Enter Your First Name: <input id="first-name"/></label>
	<label for="last-name">Enter Your Last Name: <input id="last-name"/></label>
	<label for="email">Enter Your Email: <input id="email"/></label>
	<label for="new-password">Create a New Password: <input id="new-password"/></label>
</fieldset>
```

<hr> 


## Pattern attribute to the password input element

- You can use the pattern attribute to define a regular expression that the password must match to be considered valid.
- "[a-z0-5]{8,}"
- The above is a regular expression which matches eight or more lowercase letters or the digits 0-5

<hr>

## Input type file

- This allow a user to upload a picture

<hr>
