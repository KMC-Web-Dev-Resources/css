CSS stands for Cascading Style Sheets. It describes how HTML elements are to be displayed. It controls the layout, look and feel, and the User Interface(UI) of a webpage. Let's take a look at basic CSS syntax.

``` p {color: red;} ```

The above code is a very basic example of a CSS syntax. **p** is known as a **selector** because we are selecting it by specifying it's name to style it. The actual style properties are written inside of the curly brackets. These brackets are written in opening and closing pair. Which means, all the styles written inside of a opening and closing curly braces imply to their particular selector.
The styles are written in a very common pattern. Let's take a look at the above code, the **color** text that we specified is knows as a **property**, to that property, we assign a value ("red" in the above example). We can conclude that a CSS syntax is all about **selector** { **property** : **value** }

## CSS Selectors 

A CSS selector selects the HTML elements you want to style. CSS selectors are used to "find" (or select) the HTML elements you want to style. We can divide CSS selectors into different categories, we will explore them eventually in the course.

### The CSS element Selector

The element selector selects HTML elements based on the element name.
Here, all p elements on the page will be center-aligned, with a red text color: 

``` 
p {
  text-align: center;
  color: red;
}
```

### The CSS id Selector

The id selector uses the id attribute of an HTML element to select a specific element. The id of an element is unique within a page, so the id selector is used to select one unique element! To select an element with a specific id, write a hash (#) character, followed by the id of the element.

The CSS rule below will be applied to the HTML element with id="para1": 

```
#para1 {
  text-align: center;
  color: red;
}
```

> Note: An id name cannot start with a number!

## CSS Comments

CSS comments are not displayed in the browser, but they can help document your source code. Comments are used to explain the code, and may help when you edit the source code at a later date. Comments are ignored by browsers. A CSS comment starts with /* and ends with */
You can add comments wherever you want in the code:

```
p {
  color: red;  /* Set text color to red */
}
```

Comments can also span multiple lines: 

```
/* This is
a multi-line
comment */

p {
  color: red;
}
```

## CSS Colors

Colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values. 

### CSS RGB Colors

An RGB color value represents RED, GREEN, and BLUE light sources.

### RGB Value

In CSS, a color can be specified as an RGB value, using this formula:

***rgb(red, green, blue)***

Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.

For example, rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255) and the others are set to 0.

To display black, set all color parameters to 0, like this: rgb(0, 0, 0).

To display white, set all color parameters to 255, like this: rgb(255, 255, 255).

### CSS HEX Colors

A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color.

### HEX Value

In CSS, a color can be specified using a hexadecimal value in the form:

**#rrggbb**

Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00). for eg : **#ff6347** is a hex value for a ***redish*** color.

> Note: We won't be discussing about **HSL**

## CSS Backgrounds

The CSS background properties are used to add background effects for elements.

### CSS background-color

The background-color property specifies the background color of an element. The background color of a page is set like this:

```
body {
  background-color: lightblue;
}
```

You can set the background color for any HTML elements:

```
h1 {
  background-color: green;
}

div {
  background-color: lightblue;
}

p {
  background-color: yellow;
}
```

### Opacity 

The **opacity** property specifies the opacity/transparency of an element. It can take a value from 0.0 - 1.0. The lower value, the more transparent:

```
div {
  background-color: green;
  opacity: 0.3;
}
```

## CSS Borders

The CSS border properties allow you to specify the style, width, and color of an element's border.

### CSS Border Style

The **border-style** property specifies what kind of border to display.

The following values are allowed:

1) **dotted** - Defines a dotted border
2) **dashed** - Defines a dashed border
3) **solid** - Defines a solid border
4) **double** - Defines a double border
5) **groove** - Defines a 3D grooved border. The effect depends on the border-color value
6) **ridge** - Defines a 3D ridged border. The effect depends on the border-color value
7) **inset** - Defines a 3D inset border. The effect depends on the border-color value
8) **outset** - Defines a 3D outset border. The effect depends on the border-color value
9) **none** - Defines no border
10) **hidden** - Defines a hidden border

## CSS Margins

Margins are used to create space around elements, outside of any defined borders. The CSS margin properties are used to create space around elements, outside of any defined borders.

With CSS, you have full control over the margins. There are properties for setting the margin for each side of an element (top, right, bottom, and left).

### Margin - Individual Sides

CSS has properties for specifying the margin for each side of an element:

- margin-top
- margin-right
- margin-bottom
- margin-left

All the margin properties can have the following values:

- auto - the browser calculates the margin
- length - specifies a margin in px, pt, cm, etc.
- % - specifies a margin in % of the width of the containing element
- inherit - specifies that the margin should be inherited from the parent element

> Note: Negative values are allowed.

Set different margins for all four sides of a **p** element:

```
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```

## CSS Padding

Padding is used to create space around an element's content, inside of any defined borders.The CSS padding properties are used to generate space around an element's content, inside of any defined borders.

With CSS, you have full control over the padding. There are properties for setting the padding for each side of an element (top, right, bottom, and left).

### Padding - Individual Sides

- padding-top
- padding-right
- padding-bottom
- padding-left

Set different padding for all four sides of a **div** element:  

```
div {
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
```

## Conclusion

These were some of the basic examples of a few CSS properties. Remember, CSS is a vast topic and you might get overwhelmed seeing that there are so many properties and many different ways of doing things, but that is totally okay. All you need to know is that there are many things we can do in CSS and it's very handy, when you are writing CSS you are not expected to to remember every single property. One of the advantage of being a programmer is that you can google as much as you want, if you want to align a text into the center but you are getting confused regarding whether the CSS property for doing that was **font-align** or **text-align**,  don't worry, that happens to the best of use,  you can simply google :). The thing is, you only need to know about the syntax and possibilities of CSS.
