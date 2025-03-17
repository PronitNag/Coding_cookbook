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
        
        display: grid;

        This transforms it into a grid container,
        which by default displays content in a 
        single column.

    Step 3
        We want our content to be side-by-side, 
        and to do that in a grid, we need to do
        two things: 
            - specify the number of columns we want
            - specify the width of those columns

        We can accomplish both of those together
        by using the grid-template-columns property.

        Each value provided to this property
        (separated by spaces, not commas)
        will define a new column with the specified
        width.

    That's it! There is actually quite a bit more we
    could configure in our grid, but if all we want is
    two columns of content, that's all we need!
    
    We also added background colors below 
    so you can see the boundaries of the column boxes.
*/

#two-columns {
    /* STEP 2 */
    display: grid;

    /* STEP 3 */
    /*
        The grid-template-columns property values
        can use any of the existing absolute or 
        relative units we've used before.

        However, a particularly handy unit for grids
        is a new one called a "fractional unit".

        Fractional units use the suffix 'fr', and 
        function similarly to the flex property in
        flexbox containers:

        All the fractional units get added up, and 
        that sum is added to the bottom of those
        values to create fractions.

        However, if you only have one fractional
        unit, as we do below, then that simply means
        that the column defined by the fractional unit
        will take up all the remaining available space.

        So the code below will create two columns: 
            - one with a width of 250px
            - one with a flexible width that takes up
                all the remaining available space
    */
    grid-template-columns: 250px 1fr;
}

#sidebar-content {
    background-color: lightgreen;
}

#main-content {
    background-color: #37d37b;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Two Columns - Sidebar (grid)</title>
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
                <h1>Two Columns - Sidebar (grid)</h1>
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
