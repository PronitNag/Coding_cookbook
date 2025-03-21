```css
/*
    Page layout setup
*/
* {
    box-sizing: border-box
}

body {
    margin: 0px;
    font-family: sans-serif;
}

#layout {
    max-width: 800px;
    margin: 48px auto;
    text-align: center;
}

/* 
    Gallery setup 
*/
.cropped-grid-gallery {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;

    /*
        optional extra properties,
        customize as necessary
    */
    padding: 24px;
    border: 10px solid #333333;
}

.cropped-grid-gallery img {
    width: 100%;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Gallery - Cropped (grid)</title>
        <link href="css/page0.css" rel="stylesheet">
    </head>
    <body>
        <div id="layout">
            <h1>Gallery - Cropped (grid)</h1>
            <p>
                When a gallery using CSS Grid has images of 
                different aspect ration or dimensions, <br>the 
                result is usually not great.
            </p>
            <h3>Mixed Gallery</h3>
            <div class="cropped-grid-gallery">
                <img src="images/coffee_L1.jpg" alt="coffee">
                <img src="images/coffee_P1.jpg" alt="coffee">
                <img src="images/coffee_S3.jpg" alt="coffee">
                <img src="images/coffee_L3.jpg" alt="coffee">
                <img src="images/coffee_P4.jpg" alt="coffee">
                <img src="images/coffee_S1.jpg" alt="coffee">
                <img src="images/coffee_L4.jpg" alt="coffee">
                <img src="images/coffee_S2.jpg" alt="coffee">
                <img src="images/coffee_L2.jpg" alt="coffee">
            </div>
        </div>
    </body>
</html>
```
