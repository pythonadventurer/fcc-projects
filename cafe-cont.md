# Step 54
That looks better. Now try to add the same 20px padding to the top and bottom of the menu.

# Step 55
Since all 4 sides of the menu have the same internal spacing, go ahead and delete the four properties and use a single padding property with the value 20px.

# Step 56
The current width of the menu will always take up 80% of the body element's width. On a very wide screen, the coffee and dessert appear far apart from their prices.

Add a max-width property to the menu class with a value of 500px to prevent it from growing too wide.

# Step 57
You can change the font-family of text, to make it look different from the default font of your browser. Each browser has some common fonts available to it.

Change all the text in your body, by adding a font-family property with the value sans-serif. This is a fairly common font that is very readable.

# Step 58
It is a bit boring for all the text to have the same font-family. You can still have the majority of the text sans-serif and make just the h1 and h2 elements different using a different selector.

Style both the h1 and the h2 elements using a single selector so that these elements' text use Impact font.

# Step 59
You can add a fallback value for the font-family by adding another font name separated by a comma. Fallbacks are used in instances where the initial is not found/available.

Add the fallback font serif after the Impact font.

# Step 60
Make the Est. 2020 text italicized by creating an established class selector and giving it the font-style property with the value italic.

# Step 61
Now apply the established class to the Est. 2020 text.

# Step 62
The typography of heading elements (e.g. h1, h2) is set by default values of users' browsers.

Add two new type selectors (h1 and h2). Use the font-size property for both, but use the value 40px for the h1 and 30px for the h2.
