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
  


