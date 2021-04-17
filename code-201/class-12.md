# Charts.js
- first we need to download chart.js 
- then write `<canvas >` tag in html 
- than in js write your script theat include document.get statement and style your chart using css.
- attributes used with canvas:
    - id
    - width
    - hight
- At first sight a `<canvas>` looks like the `<img> `element, with the only clear difference being that it doesn't have the src and alt attributes. I
- he canvas will initially be 300 pixels wide and 150 pixels high.
- The `<canvas>` element can be styled just like any normal image 
- ex:
` <canvas id="graph" width="150" height="150">`
- closing canvas tag is mandetory .
- canvasd only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths.
- draw rectangule functions:
    - `fillRect(x, y, width, height)`
    -  or `strokeRect(x, y, width, height) `
    - or `clearRect(x, y, width, height)`
- Drawing paths:
    - you create the path.
    - use drawing commands to draw into the path.
    - nce the path has been created, you can stroke or fill the path to render it.
    - draw path functions:
        - beginPath()
        - Path methods
        - closePath()
        - stroke()
        - fill()
    - start with beginPath() and end with  closePath()-optional-.
- colors: we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
``` 
tx.fillStyle = 'orange';
ctx.fillStyle = '#FFA500';
ctx.fillStyle = 'rgb(255, 165, 0)';
ctx.fillStyle = 'rgba(255, 165, 0, 1)'; 
```
- this function for transparency: 
` globalAlpha = transparencyValue`
- Drawing text: 
    - The canvas rendering context provides two methods to render text:
        - `fillText(text, x, y [, maxWidth]) `
        - ` strokeText(text, x, y [, maxWidth]) `
    text styling  propereties:
        - font = value
        - textAlign = value
        - textBaseline = value
        - direction = value
    
