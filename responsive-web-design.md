# Learn HTML by Building a Cat Photo App

## Step 1 HTML Elements
HTML elements have opening tags like ``<h1>`` and closing tags like ``</h1>``. The text an element will display goes between its opening and closing tags.

```html
<h1>CatPhotoApp</h1>
```

## Step 2 Heading Helements
The h1 through h6 heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so h2 elements have less importance than h1 elements.

```html
<h1>CatPhotoApp</h1>
<h2>Cat Photos</h2>
```

## Step 3 The p Element
The p element is used to create a paragraph of text on websites. 
```html
   <h2>Cat Photos</h2>
    <p>Everyone loves cute cats online!</p>
```    

## Step 4 HTML Comments
Commenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with <!--, contains any number of lines of text, and ends with -->.

Here is an example of a comment with the TODO: Remove h1:

*Example Code*

<!-- TODO: Remove h1 -->

```html
<!-- TODO: Add link to cat photos -->
<p>Everyone loves cute cats online!</p>
```

## Step 5 The main Element
HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

The main element is used to represent the main content of the body of an HTML document. Content inside the main element should be unique to the document and should not be repeated in other parts of the document.

*Example Code*

html```
<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>
```

```html
   <main>
    <h1>CatPhotoApp</h1>
    <h2>Cat Photos</h2>
    <!-- TODO: Add link to cat photos -->
    <p>Everyone loves cute cats online!</p>
    </main>
```
## Step 6 Nesting and Indentation
In the previous step, you put the h1, h2, comment, and p elements inside the main element. This is called nesting. Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.

Here is an example of nesting and indentation:

*Example Code*

<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>

## Step 7 Add Images using img
You can add images to your website by using the img element. img elements have an opening tag without a closing tag. An element without a closing tag is known as a void element.

```html
 <p>Everyone loves cute cats online!</p>
 <img>
```

## Step 8 HTML Attributes
HTML attributes are special words used inside the opening tag of an element to control the element's behavior. The src attribute in an img element specifies the image's URL (where the image is located).

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
```

## Step 9 The alt Attribute
All img elements should have an alt attribute. The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.

Here is an example of an img element with an alt attribute:

*Example Code*

```html
<img src="cat.jpg" alt="A cat">
```

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back">
```

## Step 10 Anchor Element
You can link to another page with the anchor (a) element.
Here is an example linking to https://www.freecodecamp.org:

*Example Code*
```html
<a href="https://www.freecodecamp.org"></a>
```

```html
<p>Everyone loves cute cats online!</p>
<a href="https://freecatphotoapp.com"</a>
```

## Step 11 Link Text
A link's text must be placed between the opening and closing tags of an anchor (a) element.

Here is an example of a link with the text click here to go to freeCodeCamp.org:

*Example Code*
```html
<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>
```

```html
<a href="https://freecatphotoapp.com">cat photos</a>
```
## Step 12 Link Text cont'd

```html
See more <a href="https://freecatphotoapp.com">cat photos</a> in our gallery
```

## Step 13 Link Text in Paragraph
Add p tags to turn See more <a href="https://freecatphotoapp.com">cat photos</a> in our gallery. into a paragraph.

```html
<p>See more <a href="https://freecatphotoapp.com">cat photos</a> in our gallery.<p>
```

## Step 14 Anchor Element

Turn the existing text cute cats into an anchor element that links to https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg

```html
<p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
```

## Step 15 Open Link in New Tab

To open links in a new tab, you can use the `target` attribute on the anchor (`a`) element.

The `target` attribute specifies where to open the linked document. `target="_blank"` opens the linked document in a new tab or window.

Here is the basic syntax for an `a` element with a `target` attribute:

*Example Code*

```html
<a href="https://www.freecodecamp.org" target="_blank">freeCodeCamp</a>
```

Add a `target` attribute with the value `_blank` to the anchor (`a`) element's opening tag, so that the link opens in a new tab.

```html
<p>See more <a href="https://freecatphotoapp.com" target="_blank">cat photos</a> in our gallery.</p>
```

## Step 16 Remove Comment

Now that you have added the link you can remove the comment.

```html
      <!-- TODO: Add link to cat photos -->
<p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>

<p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
```

## Step 17 Turn Image into a Link

In previous steps you used an anchor element to turn text into a link. Other types of content can also be turned into a link by wrapping it in anchor tags.

Here is an example of turning an image into a link:

*Example code:*

<a href="example-link">
  <img src="image-link.jpg" alt="A photo of a cat.">
</a>

```html
      <a href="https://freecatphotoapp.com">
        <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back.">
      </a>
```

## Step 18 The section element
Before adding any new content, you should make use of a section element to separate the cat photos content from the future content.

The section element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document. It is a semantic element that helps with SEO and accessibility.

```html
    <main>

      <h1>CatPhotoApp</h1>
      
      <section>
      <h2>Cat Photos</h2>
      <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
      <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
      <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
    </main>
```

## Step 19 Add a new section

```html
      <section>
        <h2>Cat Photos</h2>
        <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
    <section>
      </section> 
```

## Step 20 Add h2 to new section

```html
      <section>
        <h2>Cat Lists</h2>
      </section>
```

## Step 21 Implied subsection

When you add a lower rank heading element to the page, it's implied that you're starting a new subsection.

After the last h2 element of the second section element, add an h3 element with this text:

Things cats love:

```html
     <section>
        <h2>Cat Lists</h2>
          <h3>Things cats love:</h3>
      </section>
```

## Step 22 Unordered Lists

To create an unordered list of items, you can use the ul element.

After the h3 element with the Things cats love: text, add an unordered list (ul) element. Note that nothing will be displayed at this point.

```html
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul></ul>
```

## Step 23 The list item element

```html
        <ul>
          <li>cat nip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
          
        </ul>
```

## Step 24 Add an image and alt attribute

```html
        <ul>
          <li>cat nip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
        <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
```

## Step 25 The figure element
The figure element represents self-contained content and will allow you to associate an image with a caption.

```html
       <figure> <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
      </figure>
```

## Step 26 Figure caption
A figure caption (figcaption) element is used to add a caption to describe the image contained within the figure element.

```html
  <figure>
    <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
    <figcaption>Cats love lasagna.</figcaption>  
  </figure>
```

## Step 27 Emphasis
To place emphasis on a specific word or phrase, you can use the em element.

```html
<figcaption>Cats <em>love</em> lasagna.</figcaption>

```

## Step 28 Add h3 element

```html
 <h3>Top 3 things cats hate:</h3>
```



## Step 

```html

```