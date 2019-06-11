# CSS
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

## Colors
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
