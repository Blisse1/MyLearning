<hr>

Tags: #html/inputs

<hr>

- The input element allows you several ways to collect data from a web form.

- Input elements are self-closing.

There are many kinds of inputs you can create using *type attribute*

```html
<!-- Input to get text from user -->
<input type="text"> 
```

<hr>

#### Radio button input element

- If you select the ***Indoor radio button*** and submit the form, the ***form data for the button*** is based on its ***name*** and ***value*** attributes. 
- Since your radio buttons do not have a value attribute, the form data will include "*indoor-outdoor=on*", which is not useful when you have multiple buttons. 
- Add a value attribute to both radio buttons. For convenience, set the button's value attribute to the same as its id attribute.

```html
<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
```

#html/radio-input

<hr>
