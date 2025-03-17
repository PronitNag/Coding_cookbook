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
    with a center column:
    
    Step 1 
        Start by setting an explicit width.
        Either absolute or relative units are fine
        (although you'll probably also want to set
        a min-width if using relative units,
        as we do below).
    
    Step 2
        Next, set the auto value on the left/right 
        margin of the column.

        You can use the margin shorthand
        (margin: top/bottom left/right),

        or the individual margin side properties
        (
            margin-left: auto; 
            margin-right: auto;
        )

    That's it! We also added a background
    color below so you can see the boundaries
    of the column.
*/

.center-column {
    background-color: lightblue;

    /* Step 1 */
    width: 50%; 
    min-width: 500px;

    /* Step 2 */
    margin: 0px auto; 
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Single Column - Center (margin)</title>
        <link href="css/basic.css" rel="stylesheet">
    </head>
    <body>
        <div class="center-column">
            <h1>Single Column - Center (margin)</h1>
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
