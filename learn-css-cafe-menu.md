# Learn CSS By Building a Cafe Menu

## Step 8
There will be two sections on the menu, one for coffees and one for desserts. Add a section element within the main element so you have a place to put all the coffees available.

```html
<main>
  <h1>CAMPER CAFE</h1>
  <p>Est. 2020</p>
</main>
```

## Step 9
n h2 element in the section element and give it the text Coffee.

## Step 10
Up until now, you have been limited regarding the presentation and appearance of the content you create. To start taking control, add a style element within the head element.

## Step 11
You can add style to an element by specifying it in the style element and setting a property for it like this:

element {
 property: value;
}

Center the content of the h1 element by setting its text-align property to the value center

## Step 12
In the previous step, you used a type selector to style the h1 element. Center the content of the h2 and the p elements by adding a new type selector for each one to the existing style element.

## Step 13
You now have three type selectors with the exact same styling. You can add the same group of styles to many elements by creating a list of selectors. Each selector is separated with commas like this:
Example Code

selector1, selector2 {
  property: value;
}

Delete the three existing type selectors and replace them with one selector list that centers the text for the h1, h2, and p elements.


## Step 14
You have styled three elements by writing CSS inside the style tags. This works, but since there will be many more styles, it's best to put all the styles in a separate file and link to it.

We have created a separate styles.css file for you and switched the editor view to that file. You can change between files with the tabs at the top of the editor.

Start by rewriting the styles you have created into the styles.css file. Make sure to exclude the opening and closing style tags.


## Step 15
Now that you have the CSS in the styles.css file, go ahead and remove the style element and all its content. Once it is removed, the text that was centered will shift back to the left.

## Step 16
Now you need to link the styles.css file, so the styles will be applied again. Inside the head element, add a link element. Give it a rel attribute with the value of "stylesheet" and an href attribute with the value of "styles.css".

## Step 17
For the styling of the page to look similar on mobile as it does on a desktop or laptop, you need to add a meta element with a special content attribute.

Add the following within the head element:
Example Code

<meta name="viewport" content="width=device-width, initial-scale=1.0" />

## Step 18
The text is centered again so the link to the CSS file is working. Add another style to the file that changes the background-color property to brown for the body element.

## Step 19
That brown background makes it hard to read the text. Change the body element's background color to be burlywood so it has some color but you are still be able to read the text.

## Step 20
The div element is used mainly for design layout purposes unlike the other content elements you have used so far. Add a div element inside the body element and then move all the other elements inside the new div.

Inside the opening div tag, add the id attribute with a value of menu.

## Step 21
The goal now is to make the div not take up the entire width of the page. The CSS width property is perfect for this.

You can use the id selector to target a specific element with an id attribute. An id selector is defined by placing the hash symbol # directly in front of the element's id value. For example, if an element has the id of cat then you would target that element like this:
Example Code

#cat {
  width: 250px;
}

## Step 22
Comments in CSS look like this:

/* comment here */

In your style sheet, comment out the line containing the background-color property and value, so you can see the effect of only styling the #menu element. This will make the background white again.

## Step 23
Now use the existing #menu selector to set the background color of the div element to be burlywood.

## Step 24
Now it's easy to see that the text is centered inside the #menu element. Currently, the width of the #menu element is specified in pixels (px).

Change the width property's value to be 80%, to make it 80% the width of its parent element (body).

## Step 25
Next, you want to center the #menu horizontally. You can do this by setting its margin-left and margin-right properties to auto. Think of the margin as invisible space around an element. Using these two margin properties, center the #menu element within the body element.

## Step 26
So far you have been using type and id selectors to style elements. However, it is more common to use a different selector to style your elements.

A class selector is defined by a name with a dot directly in front of it, like this:
Example Code

.class-name {
  styles
}

Change the existing #menu selector into a class selector by replacing #menu with a class named .menu.

## Step 27
To apply the class's styling to the div element, remove the id attribute and add a class attribute to the div element's opening tag. Make sure to set the class value to menu.


## Step 28
Since the cafe's main product for sale is coffee, you could use an image of coffee beans for the background of the page.

Delete the comment and its contents inside the body type selector. Now add a background-image property and set its value to url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg).

## Step 29
It’s looking good. Time to start adding some menu items. Add an empty article element under the Coffee heading. It will contain a flavor and price of each coffee you currently offer.

## Step 30
article elements commonly contain multiple elements that have related information. In this case, it will contain a coffee flavor and a price for that flavor. Nest two p elements inside your article element. The first one's text should be French Vanilla, and the second's text 3.00.

## Step 31
Starting below the existing coffee/price pair, add the following coffee and prices using article elements with two nested p elements inside each. As before, the first p element's text should contain the coffee flavor and the second p element's text should contain the price.

## Step 32
The flavors and prices are currently stacked on top of each other and centered with their respective p elements. It would be nice if the flavor was on the left and the price was on the right.

Add the class name flavor to the French Vanilla p element.

## Step 33
Using your new flavor class as a selector, set the text-align property's value to left.

## Step 34

## Step 35
Now align the text to the right for the elements with the price class.

## Step 36
That is kind of what you want, but now it would be nice if the flavor and price were on the same line. p elements are block-level elements, so they take up the entire width of their parent element.

To get them on the same line, you need to apply some styling to the p elements so they behave more like inline elements. To do that, start by adding a class attribute with the value item to the first article element under the Coffee heading.

## Step 37
The p elements are nested in an article element with the class attribute of item. You can style all the p elements nested anywhere in elements with a class named item like this:

Example Code

.item p { }

Using the above selector, add a display property with value inline-block so the p elements behave more like inline elements.

## Step 38
That's closer, but the price didn't stay over on the right. This is because inline-block elements only take up the width of their content. To spread them out, add a width property to the flavor and price class selectors that have a value of 50% each.

## Step 39
Well that did not work. Styling the p elements as inline-block and placing them on separate lines in the code creates an extra space to the right of the first p element, causing the second one to shift to the next line. White space characters can cause this issue as well.

One way to fix this is to make each p element's width a little less than 50%. Change the width value to 49% for each class to see what happens.

## Step 40
That worked, but there is still a little space on the right of the price.

You could keep trying various percentages for the widths. Instead, use the back space key on your keyboard to move the p element with the class price next to the p element with the class flavor so that they are on the same line in the editor. Make sure there is no space between the two elements.

## Step 41
Now go ahead and change both the flavor and price class' widths to be 50% again.

## Step 42
Now that you know it works, you can change the remaining article and p elements to match the first set. Start by adding the class item to the other article elements.

## Step 43
Next, position the other p elements to be on the same line with no space between them.

## Step 44
To complete the styling, add the applicable class names flavor and price to all the remaining p elements.

## Step 45
If you make the width of the page preview smaller, you will notice at some point, some of the text on the left starts wrapping around to the next line. This is because the width of the p elements on the left side can only take up 50% of the space.

Since you know the prices on the right have significantly fewer characters, change the flavor class width value to be 75% and the price class width value to be 25%.

## Step 46
You will come back to styling the menu in a few steps, but for now, go ahead and add a second section element below the first for displaying the desserts offered by the cafe.

## Step 47
Add an h2 element in the new section and give it the text Desserts.

## Step 48
## Step 49
## Step 50
## Step 51
## Step 52
## Step 53
## Step 54
## Step 55
## Step 56
## Step 57
## Step 58
## Step 59
## Step 60
## Step 61
## Step 62
## Step 63
## Step 64
## Step 65
## Step 66
## Step 67
## Step 68
## Step 69
## Step 70
## Step 71
## Step 72


