# [CSS](https://www.w3schools.com/css/default.asp)

## Go to
- [Syntax](#syntax)
- [Selector](#selector)
- [Comments](#comments)
- [CSS How To](#css-how-to)
- [Cascading Order](#cascading-order)
- [Colors](#colors)
- [Backgrounds](#backgrounds)
- [Borders](#borders)
- [Margins](#margins)
- [Padding](#padding)
- [Height and Width](#height-and-width)
- [Box Model](#box-model)
- [Outline](#outline)
- [Text](#text)

## Syntax
```
h1 {color:blue; font-size:12px}
```
> selector {Property: value}

## Selector
- id: #h1
- class: .test
- grouping: 
  ```
  h1, h2, p {
    text-align: center;
  }
  ```
  
 ## Comments
> /* This is a single-line comment */
  
 ## CSS How To
- External style sheet
```
  <head>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
  </head>
```
- Internal style sheet
```
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
</style>
</head>
```
- Inline style
```
<h1 style="color:blue;margin-left:30px;">This is a heading</h1>
```

## Cascading Order
1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default

## [Colors](https://www.w3schools.com/css/css_colors.asp)
[HTML supports 140 standard color names.](https://www.w3schools.com/colors/colors_names.asp)
- RGB Value:
    `rgb(0~255, 0~255, 0~255)`
- Hax Value:
   `#rrggbb`
   > Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).
- HSL Value:
  `hsl(hue, saturation, lightness)`
- RGBA Value:
  `rgba(red, green, blue, alpha)`
- HSLA Value:
  `hsla(hue, saturation, lightness, alpha)`

## [Backgrounds](https://www.w3schools.com/css/css_background.asp)
- background-color
```
body {
  background-color: lightblue;
}
```
- background-image
```
body {
  background-image: url("paper.gif");
}
```
- Background Image - Repeat Horizontally or Vertically
```
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x / repeat-x / no-repeat ;
}
```
- Background Image - Set position and no-repeat
```
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```
- Background Image - Fixed position
```
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
```
- Background - Shorthand property
```
body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}
```

- Other background property
  - background-clip
  > The background-clip property defines how far the background (color or image) should extend within an element.
  ```
  div {
    border: 10px dotted black;
    padding: 15px;
    background: lightblue;
    background-clip: padding-box/ border-box/ content-box;
  }
  ```
  
  - [background-origin](https://www.w3schools.com/cssref/css3_pr_background-origin.asp)
  - [background-size](https://www.w3schools.com/cssref/css3_pr_background-size.asp)
  ```
  #example1 {
  background: url(mountain.jpg);
  background-repeat: no-repeat;
  background-size: auto;
  }
  ```
  ```
  #example2 {
    background: url(mountain.jpg);
    background-repeat: no-repeat;
    background-size: 300px 100px;
  }
  ```
  
## [Borders](https://www.w3schools.com/css/css_border.asp)
- Border Style
  - dotted - Defines a dotted border
  - dashed - Defines a dashed border
  - solid - Defines a solid border
  - double - Defines a double border
  - groove - Defines a 3D grooved border. The effect depends on the border-color value
  - ridge - Defines a 3D ridged border. The effect depends on the border-color value
  - inset - Defines a 3D inset border. The effect depends on the border-color value
  - outset - Defines a 3D outset border. The effect depends on the border-color value
  - none - Defines no border
  - hidden - Defines a hidden border
  ```
  p.mix {border-style: dotted dashed solid double;}
  ```
- Border Width
```
p.three {
  border-style: solid;
  border-width: 2px 10px 4px 20px;
}
```

- Border Color
```
p.three {
  border-style: solid;
  border-color: red green blue yellow;
}
```

- Individual Sides
> (top, right, bottom, left)
> (top, right/left, bottom)
> (top/bottom, right/left)
> (four sides)

- Shorthand Property
```
p {
  border: 5px solid red;
}
```
```
p {
  border-left: 6px solid red;
  background-color: lightgrey;
}
```

- Rounded Borders
```
p {
  border: 2px solid red;
  border-radius: 5px;
}
```

- other property

| Property	| Description |
| --- | --- |
|border|	Sets all the border properties in one declaration|
|border-bottom	|Sets all the bottom border properties in one declaration|
|border-bottom-color|	Sets the color of the bottom border|
|border-bottom-style|	Sets the style of the bottom border|
|border-bottom-width|	Sets the width of the bottom border|
|border-color|	Sets the color of the four borders|
|border-left|	Sets all the left border properties in one declaration|
|border-left-color|	Sets the color of the left border|
|border-left-style	|Sets the style of the left border|
|border-left-width|	Sets the width of the left border|
|border-radius	|Sets all the four border-*-radius properties for rounded corners|
|border-right	| Sets all the right border properties in one declaration|
|border-right-color|	Sets the color of the right border|
|border-right-style|	Sets the style of the right border|
|border-right-width|	Sets the width of the right border|
|border-style|	Sets the style of the four borders|
|border-top|	Sets all the top border properties in one declaration|
|border-top-color|	Sets the color of the top border|
|border-top-style|	Sets the style of the top border|
|border-top-width|	Sets the width of the top border|
|border-width|	Sets the width of the four borders|



## [Margins](https://www.w3schools.com/css/css_margin.asp)

> The CSS margin properties are used to create space around elements, outside of any defined borders.

- Individual Sides
  - margin-top
  - margin-right
  - margin-bottom
  - margin-left
  
- Shorthand Property
```
p {
  margin: 25px 50px 75px 100px;
}
```

- The auto Value

> The element will then take up the specified width, and the remaining space will be split equally between the left and right margins:

```
div {
  width: 300px;
  margin: auto;
  border: 1px solid red;
}
```

- The inherit Value

> This example lets the left margin of the <p class="ex1"> element be inherited from the parent element (<div>):
  
```
<div>
  <p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
</div>
  
div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
```

- Margin Collapse

> Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.

  This does not happen on left and right margins! Only top and bottom margins!

```
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
</style>
</head>
<body>

<p>In this example the h1 element has a bottom margin of 50px and the h2 element has a top margin of 20px. Then, the vertical margin between h1 and h2 should have been 70px (50px + 20px). However, due to margin collapse, the actual margin ends up being 50px.</p>

<h1>Heading 1</h1>
<h2>Heading 2</h2>

</body>
</html>
```

## Padding

> The CSS padding properties are used to generate space around an element's content, inside of any defined borders.

- Individual Sides
  - padding-top
  - padding-right
  - padding-bottom
  - padding-left
  
  ```
  div {
    padding-top: 50px;
    padding-right: 30px;
    padding-bottom: 50px;
    padding-left: 80px;
  }
  ```
 
- Shorthand Property
```
div {
  padding: 25px 50px 75px 100px;
}
```

- [CSS Box Model](https://www.w3schools.com/css/css_boxmodel.asp)

- Padding and Element Width
```
<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 300px;
  background-color: yellow;
}

div.ex2 {
  width: 300px;
  padding: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Padding and element width</h2>

<div class="ex1">This div is 300px wide.</div>
<br>

<div class="ex2">The width of this div is 350px, even though it is defined as 300px in the CSS.</div>

</body>
</html>
```

## [Height and Width](https://www.w3schools.com/css/css_dimension.asp)

> The height and width properties do not include padding, borders, or margins; they set the height/width of the area inside the padding, border, and margin of the element!

- Setting max-width
```
div {
  max-width: 500px;
  height: 100px;
  background-color: powderblue;
}
```

> **Note**: The value of the max-width property overrides width.


## [Box Model](https://www.w3schools.com/css/css_boxmodel.asp)

```
div {
  width: 320px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0; 
}
```
Here is the calculation:

```
320px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px
```

The total width of an element should be calculated like this:

Total element width = width + left padding + right padding + left border + right border + left margin + right margin

The total height of an element should be calculated like this:

Total element height = height + top padding + bottom padding + top border + bottom border + top margin + bottom margin


## [Outline](https://www.w3schools.com/css/css_outline.asp)

- outline properties
  - outline-style
  - outline-color
  - outline-width
  - outline-offset
  - outline

> Note: Outline differs from borders! Unlike border, the outline is drawn outside the element's border, and may overlap other content. Also, the outline is NOT a part of the element's dimensions; the element's total width and height is not affected by the width of the outline.

- Outline Style
  - dotted - Defines a dotted outline
  - dashed - Defines a dashed outline
  - solid - Defines a solid outline
  - double - Defines a double outline
  - groove - Defines a 3D grooved outline
  - ridge - Defines a 3D ridged outline
  - inset - Defines a 3D inset outline
  - outset - Defines a 3D outset outline
  - none - Defines no outline
  - hidden - Defines a hidden outline
  
```
p.ex1 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
}
```

- Outline Width
  - thin (typically 1px)
  - medium (typically 3px)
  - thick (typically 5px)
  - A specific size (in px, pt, cm, em, etc)
 
```
 p.ex1 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thin;
}
```

- Shorthand property
```
p.ex1 {outline: dashed;}
p.ex2 {outline: dotted red;}
p.ex3 {outline: 5px solid yellow;}
p.ex4 {outline: thick ridge pink;}
```
- Outline Offset
> The outline-offset property adds space between an outline and the edge/border of an element. The space between an element and its outline is transparent.
  
  
## [Text](https://www.w3schools.com/css/css_text.asp)

- text color
```
body {
  color: blue;
}

h1 {
  color: green;
}
```

- Text Alignment

> A text can be left or right aligned, centered, or justified.

When the text-align property is set to `justify`, each line is stretched so that every line has equal width, and the left and right margins are straight (like in magazines and newspapers):

- Text Decoration

The `text-decoration` property is used to set or remove decorations from text.

The value `text-decoration: none;` is often used to remove underlines from links:

```
h1 {
  text-decoration: overline;
}

h2 {
  text-decoration: line-through;
}

h3 {
  text-decoration: underline;
}
```

- Text Transformation

```
p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
```

- Text Indentation
```
p {
  text-indent: 50px;
}
```

- Letter Spacing
> The `letter-spacing` property is used to specify the space between the characters in a text.

```
h1 {
  letter-spacing: 3px;
}

h2 {
  letter-spacing: -3px;
}
```

- Line Height

> The `line-height` property is used to specify the space between lines:

```
p.small {
  line-height: 0.8;
}

p.big {
  line-height: 1.8;
}
```

- Text Direction
The `direction` property is used to change the text direction of an element:

```
p {
  direction: rtl;
}
```

- Word Spacing

The `word-spacing` property is used to specify the space between the words in a text.

```
h1 {
  word-spacing: 10px;
}

h2 {
  word-spacing: -5px;
}
```

- Text Shadow

The following example specifies the position of the horizontal shadow (3px), the position of the vertical shadow (2px) and the color of the shadow (red):

```
h1 {
  text-shadow: 3px 2px red;
}
```





