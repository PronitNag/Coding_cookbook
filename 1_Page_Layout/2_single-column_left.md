```css
/* COMMON PAGE LAYOUT SETUP CSS - START *****************/
* {
    box-sizing: border-box;
}

body {
    margin: 0px;
    /* preferred copy font goes here */
    font-family: sans-serif; 
}
/* COMMON PAGE LAYOUT SETUP CSS - END ********************/

/*
    To create a single column layout
    with a right-aligned column:
    
    Step 1 
        Start by setting an explicit width.
        Either absolute or relative units are fine
        (although you'll probably also want to set
        a min-width if using relative units,
        as we do below).

    Step 2
        Next, set a margin-left value of auto.
        This will tell the element to shift all
        of the available empty space to the 
        left margin, effectively pushing the 
        content to the right.

    That's it! We also added a background color 
    below so you can see the boundaries of the column.
*/

.center-column {
    background-color: lightblue;

    /* Step 1 */
    width: 50%; 
    min-width: 500px;

    /* Step 2 */
    margin-left: auto;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Single Column - Right</title>
        <link href="css/basic.css" rel="stylesheet">
    </head>
    <body>
        <div class="center-column">
            <h1>Single Column - Right</h1>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Cupiditate necessitatibus ab ipsum? Natus suscipit 
                asperiores alias ipsam, cum, accusamus quisquam nam 
                magnam aspernatur vel tenetur quibusdam. Consequatur 
                itaque similique provident. Lorem ipsum dolor sit, amet 
                consectetur adipisicing elit. Iste ipsum veritatis ullam, 
                dolor tempora quo. Omnis, id pariatur. Accusantium facere 
                quo praesentium aspernatur omnis qui ratione impedit 
                aperiam minima dolorem.
            </p>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                Porro, commodi similique ipsa tempora perspiciatis, sed 
                exercitationem reprehenderit sapiente a cumque voluptates 
                veniam est, quia totam voluptatibus eaque consectetur 
                optio ipsum.
            </p>
            <h3>Lorem ipsum dolor</h3>
            <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. 
                Dolore architecto explicabo reprehenderit vel saepe, 
                illum vitae dicta tempora aperiam repellendus sed 
                aspernatur corrupti consequatur culpa ratione dolor
                tempore quas ipsa.
            </p>
        </div>
    </body>
</html>
```
