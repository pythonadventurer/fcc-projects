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
## Step 20
## Step 21
## Step 22
## Step 23
## Step 24
## Step 25
## Step 26
## Step 27
## Step 28
## Step 29
## Step 30
## Step 31
## Step 32
## Step 33
## Step 34
## Step 35
## Step 36
## Step 37
## Step 38
## Step 39
## Step 40
## Step 41
## Step 42
## Step 43
## Step 44
## Step 45
## Step 46
## Step 47
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


