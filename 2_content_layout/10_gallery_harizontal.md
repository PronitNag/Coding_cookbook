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
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Gallery - Horizontal Masonry (flex)</title>
        <link href="css/page0.css" rel="stylesheet">
    </head>
    <body>
        <div id="layout">
            <h1>Gallery - Horizontal Masonry (flex)</h1>
            <p>
                Masonry layouts are named after the construction
                approach of building a stone wall by laying
                stones of different sizes side-by-side or on 
                top of each other to create a cohesive whole.
            </p>
            <p>
                Masonry galleries are great because they can 
                usually handle images of any size or dimension,
                as we'll see after transforming the mess of
                images below into a horizontal masonry gallery.
            </p>
            <h3>Mixed Gallery</h3>
            <div class="horizontal-masonry-gallery">
                <img src="images/coffee_P3.jpg" alt="coffee">
                <img src="images/coffee_L1.jpg" alt="coffee">
                <img src="images/coffee_P1.jpg" alt="coffee">
                <img src="images/coffee_L3.jpg" alt="coffee">
                <img src="images/coffee_P4.jpg" alt="coffee">
                <img src="images/coffee_S1.jpg" alt="coffee">
                <img src="images/coffee_P3.jpg" alt="coffee">
                <img src="images/coffee_S2.jpg" alt="coffee">
                <img src="images/coffee_L2.jpg" alt="coffee">
            </div>
        </div>
    </body>
</html>
```
