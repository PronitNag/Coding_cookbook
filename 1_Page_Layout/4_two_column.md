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
    To create a two column layout
    with a left sidebar:
    
    Step 1 
        Start in the HTML by creating a container 
        element, and inside of it, put two other 
        container elements, one for the sidebar 
        content and one for the main page content.
    
    Step 2
        Next, target the outer container element and
        give it the following property and value: 
        
        display: flex;

        This transforms it into a flexbox container,
        which by default displays content in a row,
        or in other words, side-by-side.

    Step 3
        By default, each element in a flexbox will
        only take up the necessary space they need in 
        a row, so we'll need to resize the sidebar

        Set an explicit width on the sidebar; either
        absolute or relative units will work, but
        we usually want our sidebar content width
        to be constant, so I'd recommend absolute units.

    Step 4
        Now that we have a width on the sidebar,
        we need to resize the main content container
        to take up the remaining space.

        Flexbox makes this very simple by applying
        the following property to that container:
        
        flex: 1;

        That flex property is a shorthand property,
        and by providing a number, we'll tell it to
        take up all the remaining space.

        (This gets a litte more complicated if there 
        are other elements using the flex property,
        but since this is the only one, we're good)

    That's it! We also added background colors below 
    so you can see the boundaries of the column boxes.
*/

#two-columns {
    /* STEP 2 */
    display: flex;
}

#sidebar-content {
    background-color: lightgreen;
    /* STEP 3 */
    width: 250px;
}

#main-content {
    background-color: #37d37b;
    /* STEP 4 */
       flex: 1;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Two Columns - Sidebar (flex)</title>
        <link href="css/basic-left.css" rel="stylesheet">
    </head>
    <body>
        <div id="two-columns">
            <div id="sidebar-content">
                <h2>BRAND NAME</h2>
                <ul>
                    <li><a href="#">Link 1</a></li>
                    <li><a href="#">Link 2</a></li>
                    <li><a href="#">Link 3</a></li>
                    <li><a href="#">Link 4</a></li>
                </ul>
            </div>
            <div id="main-content">
                <h1>Two Columns - Sidebar (flex)</h1>
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
        </div>
    </body>
</html>
```
