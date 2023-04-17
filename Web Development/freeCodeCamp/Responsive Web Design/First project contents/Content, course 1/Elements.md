<hr>

Tags: #html/elements

<hr>

## Label element

- Label elements are used to help associate the text for an input element with the input element itself ***(especially for assistive technologies like screen readers)*** 

```html
<!-- Clicking the word cat also selects the corresponding radio button -->
<label><input type="radio"> cat</label>
```

#html/label

<hr>

## Img element (<img><"img">)

- img elements have an opening tag without a closing tag. This is called ***self-closing tag.***

- The ***src*** attribute in an img specifies the ***image's URL***. 

```html
<!-- Link directing to an image -->
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
```

- All img elements should have an ***alt*** attribute. The ***alt*** attribute's text is used for screen readers to improve accesibility and is displayed if the image ***fails*** to load.

```html
<!-- Alt attribute describing the image. -->
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back">
```

#html/img

<hr>

## Anchor element (<"a">)

- You link to another page with the anchor (a) element.

```html
<!-- Anchor tag redirecting to freecodecamp.org -->
<a href="https://freecodecamp.org"></a>
```

- A link's text must be placed between the opening and closing tags of an anchor (a) element.

```html
<!-- Text added between opening and closing tags -->
<a href="https://freecodecamp.org">This is the link!</a>
```

- You can even combine it with inside a "p" element.

```html
<!-- Specific text marked up with an anchor element.-->
<p>This is a <a href="#">test</a></p>
```

- Even with an ***img*** element
```html
<!-- Making an img element clickable -->
<a href="#"><img src="#" target="_blank"></a>
```

#html/a

<hr>

## Button element behavior in a form

- To create a clickable button 

```html
<!-- A button with the text "Click Here" -->
<button>Click Here</button>
```

- The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's action attribute.

- But we don't rely on *default behavior* because that may cause *confusion*, so we add type attribute to it to make it clear that it is a submit button.

```html
<!-- A type submit button -->
<button type="submit">Click Here</button>
```

#html/button

<hr>

## Figure element (<"figure">)

- The figure element represents self-contained content and will allow you to associate an image with a caption
- A figure caption (figcaption) element is used to add caption to describe the image contained within the figure element.

```html
<figure>
	<img src="#">
	<figcaption>There is nothing inside here!</figcaption>
</figure>
```

#html/figure

<hr>

## Fieldset element

- It is used to group related [[Inputs]] and labels together in a webform. Fieldset elements are block-level elements, meaning that they appear in a new line.

```html
<!-- Use of fieldset -->
<fieldset>
	<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
	<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
```

- The legend element acts as a caption for the content in the fieldset element. It gives user context about what they should enter into that part of the form.

```html
<!-- A legend element giving context -->
<fieldset>
	<legend>A text that gives context.</legend>
	<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
	<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
```

#html/fieldset

<hr>

## Main element

- This HTML element represents the **dominant** **content** of the body of a document.

- The main content area consists of the content that is directly related to or expands upon the central topic of a document, or the **central functionality of an application**.

```html
<!-- Example taken from MDN -->
<header>Gecko Facts</header>
<main>
    <p>Geckos are a group of usually small, usually nocturnal lizards. They are found on every continent except Australia.</p>
 
    <p>Many species of gecko have adhesive toe pads which enable them to climb walls and even windows.</p>
</main>
```

#html/main

<hr>

## Section element

- The section element represents a generic standalone section of a document.
- Sections should always have a heading, with very few exceptions.
- Should be used if there isn't a more specific element to represent it. 

```html
<!-- Example of different sections taken from MDN-->
<h1>Choosing an Apple</h1>
<section>
    <h2>Introduction</h2>
    <p>This document provides a guide to help with the important task of choosing the correct Apple.</p>
</section>

<section>
    <h2>Criteria</h2>
    <p>There are many different criteria to be considered when choosing an Apple — size, color, firmness, sweetness, tartness...</p>
</section>
```

- A navigation menu should be wrapped in a **nav element**, but a list of search results or a map display and its controls don't have specific elements, and could be put inside a **section element**.

### Important use cases

- If the contents of the element represents a standalone, atomic unit of content that makes sense syndicated as a standalone piece (e.g a blog post or blog comment, or a newspaper article) the **article element** would be a better choice. #html/article

- If the contents represent useful tangential information that works alongside the main content, but not directly part of it (like related links, or an author bio), use **an aside element**. #html/aside

- If the contents represent the main content of the area of a document, use **main element**.

- If you are only using the element as styling wrapper, use a **div** instead. #html/div

### Exceptions of sections without a heading

- Secondary navigation system:

```html
<section>
	<a href>Previous Article</a>	
	<a href>Next Article</a>	
</section>
```

```html
<section>
  <button class="reply">Reply</button>
  <button class="reply-all">Reply to all</button>
  <button class="fwd">Forward</button>
  <button class="del">Delete</button>
</section>
```

#html/section

<hr> 

## Style element

^1a6671

You can add style to an element by specifying it in the style element and setting a property for it like this:

```html
<head>
	<style>
		element {
			property: value;
		}
	</style>
</head>
```

You can add the style in the head of the HTML.

- You have styled three elements by writing CSS inside the style tag. This works, but since there will be many more styles, it's best to put all the styles in a **separate file and link to it**. 

#html/style

<hr>

## Meta element
#html/meta

^6a0eec

- For the styling of the page to look similar on mobile as it does on a desktop or laptop, you need to add a meta element with a special content attribute

```html
<!-- Meta tag to make the page look similar on mobile as it does on desktop -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- A viewport definition tells the browser how to render the page. 

<hr>

## Div element
#html/div

- The div element is used mainly for design layout purposes
- A la pregunta que tenía sobre cómo estructurar el HTML con main y aside y bien semantico con Divs, aquí está un ejemplo sobre cómo se podría hacer.

```html
<!-- Elements inside a div -->
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

<hr> 

## Article element
#html/article

- Article elements commonly contain multiple elements that have related information.
- It is intended to be independently distributable or reusable. Examples include:
<ol>
	<li>A forum post</li>
	<li>A magazine or newspaper article</li>
	<li>A blog entry </li>
	<li>Or any other independent item of content</li>
</ol>

```html
<!-- Related information -->
<article>
	<p>French Vanilla</p>
	<p>3.00</p>
</article>
```


### Usage notes
- When an article element is nested, the inner element represents an article related to the outer element. For example the comments of a blog post can be article elements nested in the article representing the blog post

```html
<!-- Nested articles with semantic meaning-->
<article class="blog-post">
	<article class="comments"></article>
</article>
```

<hr>

## Address element
#html/address

- Its an element that indicates that the enclosed HTML provides contact information for a person or people, or for an organization.

- It conveys additional semantic information.

```html
<p>Contact the author of this page:</p>
<address>
	<a href="mailto:jim@rock.com">jim@rock.com</a> 
	<a href="tel:+1455412">(311 555-2368)</a> 
</address>
```

- It can contain whatever form is appropiate for the context, and may include any type of contact information that is needed, such as:

	- physical address
	- URL 
	- email address
	- phone number 
	- social media handle 
	- geographic coordinates 

- The address element should include the name of the person, people or organization to which the contact information refers

- It can be used such as providing a business' contact information in the page header or indicating the author of an article by including an address element within the article.

```html
<article>
	<address>
		<p>You can contact the author at:</p><br>
		<a href="somedomain.com"> This domain</a>
	</address>
</article>

```


- The element should not contain more information than the contact information like a publication date (which belongs to a time element)

- An address can be placed in a footer element, if any.
- The address element does not have to contain a physical geographical location. It can be used to provide a link to the subject.

<hr>

## Time element 
#html/time

- This element represents a specific period in time. It may include the datatime attribute to translate dates into machine-readable format, allowing for better search engine results or custom features such as reminders.

- It may represent:
 - A time on a 24-hour clock.
 - A valid time duration
 - Attribute: datatime

<hr>

## P element
#html/p-element 

- P elements are block level elements, so they can take up the entire width of their parent element.

<hr> 

## Footer element
#html/footer

- This element represents a footer for it nearest ancestor sectioning content or sectioning root element. A footer typically contains information about the author of the section, copyright data or links to related documents.

```html
<!-- A footer representing it nearest ancestor sectioning content element-->

<article>
    <h1>How to be a wizard</h1>
    <ol>
        <li>Grow a long, majestic beard.</li>
        <li>Wear a tall, pointed hat.</li>
        <li>Have I mentioned the beard?</li>
    </ol>
    <footer>
        <p>© 2018 Gandalf</p>
    </footer>
</article>
```

- Enclose information about the author in an **address element** that can be included into the footer element.
- When the nearest ancestor sectioning content or sectioning root element is the body element the footer applies to the whole page.

- The footer element is a container for a collection of content that is related to the page.

<hr>

## Title element
#html/title

- The title element gives the search engine extra information about the page. 

```html
<head>
	<title>This is a title!</title>
</head>
```

<hr>

## The text area element
#html/textarea

- This element acts like an input element of type text
- This works with rows and cols attributes
- With form submissions it is useful and good practice to provide each submittable element with a name attribute. This attribute is used to identify the element in the form submission

<hr>
