```css
/* standard page layout setup */
* {
    box-sizing: border-box
}

body {
    margin: 0px;
    font-family: Arial, Helvetica, sans-serif;
}

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

/* General comparison setup */
.comparisons-container {
    text-align: center;
    margin: 60px 0px;
}

.comparisons-container h3 {
    font-size: 36px;
}


/* Comparison Layout 1 ************************************/

/*
    This implementation uses flexbox to build columns
    within the flexbox container.
*/
.comparisons-layout-1 {
    display: flex;
    justify-content: center;
}

.comparisons-layout-1 .comparison-column {
    background-color: #bfefff;
    border: 3px solid #d86fee;
    padding: 24px;
}

.comparisons-layout-1 .comparison-column h4,
.comparisons-layout-1 .comparison-column p {
    padding: 24px 48px;
}

.comparisons-layout-1 .comparison-column h4 {
    background-color: #8122ed;
    color: #bfefff;
    font-size: 24px;
    margin: 0px
}

.comparisons-layout-1 .comparison-column p {
    font-size: 18px;
    margin: 0px;
    border-top: 3px solid #8122ed;
}

.comparisons-layout-1 .comparison-column .label {
    display: block;
    font-weight: bold;
    padding-bottom: 12px;
}

/* Comparison Layout 2 ************************************/

/*
    This implementation uses flexbox again, but this time
    we use many flexbox containers to build rows.

    This requires a different HTML structure to support it.
*/
.comparisons-layout-2 {
    background-color: #3f0791;
    padding: 36px;
}

.comparison-row {
    display: flex;
    border-bottom: 3px solid #bfefff;
    color: #bfefff;
}

.comparison-row.comparison-header {
    font-weight: bold;
}

.comparison-row div {
    flex: 1;
    padding: 24px;
    font-size: 24px;
}

/* Comparison Layout 3 ************************************/

/*
    This implementation uses CSS Grid.

    This requires yet another different HTML structure 
    to support it, but it is generally the simplest 
    of the three implementations here.
*/

.comparisons-layout-3 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
}

.comparisons-layout-3 div {
    padding: 24px;
    font-size: 24px;
    border-bottom: 3px solid #3f0791;
}

.comparisons-layout-3 .label {
    font-weight: bold;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Comparison Tables</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css" integrity="sha512-xh6O/CkQoPOWDdYTDqeRdPCVd1SpvCA9XXcUnZS2FmJNp1coAFzvtCN9BmamE+4aHK8yyUHUSCcJHgXloTyT2A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
        <link href="css/style.css" rel="stylesheet" data-meal-prep>
    </head>
    <body>
        <div id="main-section">
            <div class="single-column">

                <!--
                    Comparison Layout 1

                    This example uses a flexbox container with three
                    flexbox item "columns" inside.

                    This approach guarantees that your content will
                    stay in those columns, but you'll find that the
                    content in those columns may not always stay 
                    in neat and tidy rows.
                -->
                <div class="comparisons-container">
                    <h3>Compare MAGIC SPOON to your childhood favs</h3>
                    <div class="comparisons-layout-1">
                        <div class="comparison-column">
                            <h4>MAGIC SPOON</h4>
                            <p><span class="label">PROTEIN</span> 12-14g</p>
                            <p><span class="label">NET CARBS</span> 4-5g</p>
                            <p><span class="label">SUGAR</span> 0-1g*</p>
                            <p>
                                <span class="label">GRAIN FREE</span> 
                                <i class="fa-regular fa-thumbs-up"></i>
                            </p>
                            <p>
                                <span class="label">GLUTEN FREE</span>
                                <i class="fa-regular fa-thumbs-up"></i>
                            </p>
                        </div>
                        <div class="comparison-column">
                            <h4>Froot Loops</h4>
                            <p><span class="label">PROTEIN</span> 2g</p>
                            <p><span class="label">NET CARBS</span> 32g</p>
                            <p><span class="label">SUGAR</span> 12g</p>
                            <p>
                                <span class="label">GRAIN FREE</span></span>
                                <i class="fa-regular fa-thumbs-down"></i>
                            </p>
                            <p>
                                <span class="label">GLUTEN FREE</span></span>
                                <i class="fa-regular fa-thumbs-down"></i>
                            </p>
                        </div>
                        <div class="comparison-column">
                            <h4>Reese's Puffs</h4>
                            <p><span class="label">PROTEIN</span> 2g</span></p>
                            <p><span class="label">NET CARBS</span> 21g</span></p>
                            <p><span class="label">SUGAR</span> 9g</span></p>
                            <p>
                                <span class="label">GRAIN FREE</span> 
                                <i class="fa-regular fa-thumbs-down"></i>
                            </p>
                            <p>
                                <span class="label">GLUTEN FREE</span>
                                <i class="fa-regular fa-thumbs-down"></i>
                            </p>
                        </div>
                    </div>
                </div>

                <!--
                    Comparison Layout 2

                    This example uses multiple flexbox containers
                    that make up "rows".

                    This approach guarantees that your content will
                    stay in those rows, and is better at maintaining
                    content in a nice looking grid.
                -->
                <div class="comparisons-container">
                    <h3>Compare MAGIC SPOON to your childhood favs</h3>
                    <div class="comparisons-layout-2">
                        <div class="comparison-row comparison-header">
                            <div></div>
                            <div>MAGIC SPOON</div>
                            <div>Froot Loops</div>
                            <div>Reese's Puffs</div>
                        </div>
                        <div class="comparison-row">
                            <div>PROTEIN</div>
                            <div>12-14g</div>
                            <div>2g</div>
                            <div>2g</div>
                        </div>
                        <div class="comparison-row">
                            <div>NET CARBS</div>
                            <div>4-5g</div>
                            <div>32g</div>
                            <div>21g</div>
                        </div>
                        <div class="comparison-row">
                            <div>SUGAR</div>
                            <div>0-1g*</div>
                            <div>12g</div>
                            <div>9g</div>
                        </div>
                        <div class="comparison-row">
                            <div>GRAIN FREE</div>
                            <div><i class="fa-regular fa-thumbs-up"></i></div>
                            <div><i class="fa-regular fa-thumbs-down"></i></div>
                            <div><i class="fa-regular fa-thumbs-down"></i></div>
                        </div>
                        <div class="comparison-row">
                            <div>GLUTEN FREE</div>
                            <div><i class="fa-regular fa-thumbs-up"></i></div>
                            <div><i class="fa-regular fa-thumbs-down"></i></div>
                            <div><i class="fa-regular fa-thumbs-down"></i></div>
                        </div>
                    </div>
                </div>

                <!--
                    Comparison Layout 3

                    But if our content is basically arranged in rows
                    and columns like a grid, why don't we just use
                    CSS Grid to build it?

                    Good idea! This last example uses CSS grid to
                    build its layout, and in some ways, it's the 
                    simplest of the three layouts.
                -->
                <div class="comparisons-container">
                    <h3>Compare MAGIC SPOON to your childhood favs</h3>
                    <div class="comparisons-layout-3">

                        <!-- row content -->
                        <div></div>
                        <div class="label">MAGIC SPOON</div>
                        <div class="label">Froot Loops</div>
                        <div class="label">Reese's Puffs</div>

                        <!-- row content -->
                        <div class="label">PROTEIN</div>
                        <div>12-14g</div>
                        <div>2g</div>
                        <div>2g</div>

                        <!-- row content -->
                        <div class="label">NET CARBS</div>
                        <div>4-5g</div>
                        <div>32g</div>
                        <div>21g</div>

                        <!-- row content -->
                        <div class="label">SUGAR</div>
                        <div>0-1g*</div>
                        <div>12g</div>
                        <div>9g</div>

                        <!-- row content -->
                        <div class="label">GRAIN FREE</div>
                        <div><i class="fa-regular fa-thumbs-up"></i></div>
                        <div><i class="fa-regular fa-thumbs-down"></i></div>
                        <div><i class="fa-regular fa-thumbs-down"></i></div>

                        <!-- row content -->
                        <div class="label">GLUTEN FREE</div>
                        <div><i class="fa-regular fa-thumbs-up"></i></div>
                        <div><i class="fa-regular fa-thumbs-down"></i></div>
                        <div><i class="fa-regular fa-thumbs-down"></i></div>

                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
```
