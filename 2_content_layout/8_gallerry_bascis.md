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
.basic-grid-gallery {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;

    /*
        optional extra properties,
        customize as necessary
    */
    padding: 24px;
    border: 10px solid #333333;
}

.basic-grid-gallery img {
    width: 100%;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Gallery - Basic (grid)</title>
        <link href="css/page0.css" rel="stylesheet">
    </head>
    <body>
        <div id="layout">
            <h1>Gallery - Basic (grid)</h1>
            <p>
                CSS Grid can make a pretty nice looking gallery,<br> 
                as long as all the images are the exact same
                aspect ratio / dimensions.
            </p>
            <h3>Landscape Gallery</h3>
            <div class="basic-grid-gallery">
                <img src="images/tea_L1.jpg" alt="tea">
                <img src="images/tea_L2.jpg" alt="tea">
                <img src="images/tea_L3.jpg" alt="tea">
                <img src="images/tea_L4.jpg" alt="tea">
                <img src="images/tea_L5.jpg" alt="tea">
                <img src="images/tea_L6.jpg" alt="tea">
                <img src="images/tea_L7.jpg" alt="tea">
                <img src="images/tea_L8.jpg" alt="tea">
                <img src="images/tea_L9.jpg" alt="tea">
            </div>
            <h3>Portrait Gallery</h3>
            <div class="basic-grid-gallery">
                <img src="images/tea_P1.jpg" alt="tea">
                <img src="images/tea_P2.jpg" alt="tea">
                <img src="images/tea_P3.jpg" alt="tea">
                <img src="images/tea_P4.jpg" alt="tea">
                <img src="images/tea_P5.jpg" alt="tea">
                <img src="images/tea_P6.jpg" alt="tea">
                <img src="images/tea_P7.jpg" alt="tea">
                <img src="images/tea_P8.jpg" alt="tea">
                <img src="images/tea_P9.jpg" alt="tea">
            </div>
        </div>
    </body>
</html>
```
