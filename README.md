# [CSS](https://www.w3schools.com/css/default.asp)
## Syntax
```
h1 {color:blue; font-size:12px}
```
> selector {Property: value}

## Selector:
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
  
 ## CSS How To...
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
|border-right	Sets| all the right border properties in one declaration|
|border-right-color|	Sets the color of the right border|
|border-right-style|	Sets the style of the right border|
|border-right-width|	Sets the width of the right border|
|border-style|	Sets the style of the four borders|
|border-top|	Sets all the top border properties in one declaration|
|border-top-color|	Sets the color of the top border|
|border-top-style|	Sets the style of the top border|
|border-top-width|	Sets the width of the top border|
|border-width|	Sets the width of the four borders|



