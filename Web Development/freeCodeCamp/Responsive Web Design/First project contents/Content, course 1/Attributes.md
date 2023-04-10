<hr>

Tags: #html/attributes

<hr>

- HTML attributes are special words used inside the opening tag of an element to control the element's behavior.

<hr>

## Name attribute
#html/name-attribute

- In order for a form's data *(input, or whatever is inside the form)* to be accessed by the location specified in the **action attribute**, you must give the text field a *name* attribute and asign it a value to represent the data that is being submitted.

```html
<!-- The name must represent the data that is being submitted -->
<input type="text" name="email">
```

<hr>

## Target attribute
#html/target-attribute

- We use ***target*** attribute with the value "_ blank" so that the links opens in a new tab.

```html
<p>This is an <a href="#" target="_blank">example!</a></p>
```

<hr>

## Action attribute
#html/action-attribute

- The ***action attribute*** indicates where form data should be sent.

```html
<!-- This form action tells the browser that the form data should be sent to the path /submit-url -->
<form action="/submit-url"></form>
```

<hr>

## Required attribute
#html/required-attribute

- To prevent a user from submitting your form when required information is missing, you need to add the *required* attribute to an input element.

```html
<!-- You just add the word required at the end.-->
<input type="text" name="email" required>
```

<hr>

## ID attribute
#html/id-attribute 

- It is used to identify specific HTML elements. Each ID attribute's value must be ***unique*** from all other id values for the entire page.

```html
<input id="loving" type="text" name="email" required>
```

<hr>

## Checked attribute
#html/checked-attribute

- In order to make a checkbox checked or radio button selected by default, you need to add the checked attribute to it.

```html
<!-- Checked attribute -->
<input id="loving" type="checkbox" name="personality" value="loving" checked><label for="loving">Loving</label>
```

<hr>

## Type attribute
#html/type-attribute

^2f2a8d

### With the checkbox value:

- Add the ***name attribute*** with the value **personality** to the checkbox input element.

- While you won't notice this in the browser, doing this makes it easier for a server to process your web form, especially when there are multiple checkboxes.

```html
<!-- Adding name attribute to make it easier for a server -->
<input id="loving" type="checkbox" name="personality"><label for="loving">Loving</label>
```

- Like radio buttons, form data for the selected checkboxes are ***name / value attributes*** pairs. While the ***value*** attribute is optional, its best practice to include it with any checkboxes or radio buttons on the page. For convenience, set each checkbox's value attribute to the same value as its id attribute.

```html
<!-- Adding value attribute as best practice, and setting it to the same value of the id attribute's value -->
<input id="loving" type="checkbox" name="personality" value="loving"><label for="loving">Loving</label>
```

## Type attribute in a form element (input)

- Specifying the type attribute of a form element is important for the browser to know what kind of data it should expect. If the type is not specified, the browser will default to text

```css
<label for="first-name">Enter Your First Name: <input id="first-name" type="text"/>
```

- The first input element with a type of submit is automatically set to submit its nearest parent form element

- To correctly handle the form submission, after the last fieldset element add an input element with the type attribute set to submit and the value set to Submit

```html
<input type="submit" value="Submit">
```

<hr>

## For (with labels)
#html/for-attribute

- Second way to associate an input element's text with the element itself.

- You can nest the text within a label element and add a ***for*** attribute with the same value as the input element's id attribute.

```html
<!-- For attribute use -->
<input id="loving" type="checkbox"><label for="loving">Loving</label>
```

<hr>

## Charset 
#html/charset-attribute 

- To tell the browser how to encode characters on your page, we set charset to utf-8. That is a universal character set that includes almost every character from all human languages

```html
<!-- Character setted to utf-8 -->
<meta charset="utf-8">
```

<hr>

## Method attribute 
#html/method

- The method attribute specifies how to send form-data to the URL specified in the action attribute. The form-data can be sent via a GET request as URL parameters (with method="get") or via a post request as data in the requested body (method="post")

<hr>

## Adding custom validation to the password input element
#html/min-length

- You can do this by adding a **minleght attribute** with a value of 8. Doing so prevents inputs of less than 8 characters being submitted.

```html
<input type="password" minlength="8">
```

<hr>

## Min and max attributes
#html/min-max

```html
<label>Input your age (years): <input type="number" min="13" max="120"></label>
```

<hr>