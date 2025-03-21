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

#card-section {
    background-color: #5b00ed;
    color: #bfefff;
    padding: 48px;
}

/*
    Here we make our .card-container into a flexbox
    and tell it to space out the flex items using
    justify content with space-between.

    If you'd rather the card be centered, you could
    always change justify-content to center.
*/
.card-container {
    display: flex;
    justify-content: space-between;
}

/*
    The flex: 1; below makes each card equally
    sized within the flexbox (unless the container
    gets too small, then they may get squished).

    However, if you don't want them to grow too
    wide, you may want to consider adding a 
    max-width property.
*/
.card {
    flex: 1;
    border: 3px solid #bfefff;
    padding: 36px;
    text-align: center;
    margin: 36px;
}

.card h3 {
    font-size: 36px;
    margin: 0px;
}

.card p {
    font-size: 24px;
    margin: 24px 0px 0px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Three Cards</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="card-section">
            <div class="single-column card-container">

                <div class="card">
                    <h3>High Protein  </h3>
                    <p>12g - 14g complete protein in every bowl</p>
                </div>

                <div class="card">
                    <h3>Keto-Friendly</h3>
                    <p>4g - 5g net carbs per bowl</p>
                </div>

                <div class="card">
                    <h3>Sweet & Delicious</h3>
                    <p>Tastes just like you remember, only better.</p>
                </div>

            </div>
        </div>
    </body>
</html
```
