```css
/* standard page layout setup */
* {
    box-sizing: border-box
}

body {
    margin: 0px;
    font-family: Arial, Helvetica, sans-serif;
}

/*
    This is an alternate way of setting up a
    Centered Single Column Page Layout,
    focusing on the upper and lower limits
    that the width should grow or shrink to.
*/
.single-column {
    min-width: 600px;
    max-width: 1200px;
    margin: 0px auto;
}

#main-section {
    background: 
        radial-gradient(at top left, #d86fee, #8122ed);
    padding: 48px;
}


/*
    Media and text side-by-side implementation **************
*/

/*
    As always, applying Flexbox to the container 
    of the elements we want side by side is 
    usually the way to go.

    Remember that for a Flexbox row, the
    align-items property can be used to 
    align content vertically, in this case,
    in the center of the container.
*/
.side-by-side {
    display: flex;
    align-items: center;
    margin: 48px 0px;
}

/*
    In this case, we have the image and text containers
    with equal sizes (flex: 1), but if you want the 
    image to be larger, or conversely if you want the 
    text area to be larger, you can adjust the flex 
    values assigned to each container.
*/
.side-by-side .image-container {
    flex: 1;
}

.side-by-side .text-container {
    flex: 1;
    padding: 36px;
}

/*
    This code tells the image to stretch
    to fill the container we set up
    above; this means that the image
    will be as flexible as the Flexbox
    item it is inside of.
*/
.side-by-side .image-container img {
    width: 100%;
}

.side-by-side .text-container h3 {
    font-size: 48px;
}

/* fake button styling */
.side-by-side .text-container a {
    font-size: 28px;
    font-weight: bold;
    text-decoration: none;
    display: inline-block;
    background-color: #3f0791;
    color: white;
    padding: 24px 48px;
    border-radius: 48px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Media & Text</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="main-section">
            
            <div class="single-column">

                <!--
                    Note the structure of our "side-by-side"
                    container; inside, there are two containers:
                    one for an image, and one for text.

                    This is how you can set up a "Media & Text"
                    layout.

                    Sound familiar? You used a Block of the
                    exact same name in WordPress!

                    Now you can build your own, and customize
                    it however you want!
                -->
                <div class="side-by-side">
                    <div class="image-container">
                        <img src="images/cool-boxes.webp" alt="cereal box">
                    </div>
                    <div class="text-container">
                        <h3>High protein cereal to power your days</h3>
                        <a href="#">TRY NOW</a>
                    </div>
                </div>


                <div class="side-by-side">
                    <div class="text-container">
                        <h3>A whole world of flavor</h3>
                        <a href="#">HAVE A TASTE</a>
                    </div>
                    <div class="image-container">
                        <img src="images/warm-boxes.webp" alt="cereal box">
                    </div>
                </div>

            </div>
        </div>
    </body>
</html>
```
