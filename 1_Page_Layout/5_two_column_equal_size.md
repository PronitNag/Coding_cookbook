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
    with equally sized columns:
    
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
        a row (flexbox will try to keep the heights as 
        balanced as possible).

        To keep the widths of each column equal, we
        have two options: 

        Option 1

            width: 50%;

            Setting the code above on each column will 
            set the columns equal to 50% of the width 
            of their container.

        or, we can also use:

        Option 2

            flex: 1;

            Setting this code on each column will
            basically have the same effect as using
            the width property, but we're using a flex
            property instead.  
            
            The flex values get added up between all 
            the flexbox children using the property, 
            and split between them in fractions.
            
            Since both columns have the value of 1, 
            adding them all up gives a total of 2.

            Then, the fraction for each is 
            'flex value' / 'flex sum', or 1/2 for
            our columns (in other words, 50%).

            Actually, as long as we keep the same
            flex value for both columns, the fraction
            for them will always be 1/2, due to the 
            formula above; try out others and see!

        There isn't much difference between the two
        approaches in this case; the flex shorthand 
        property tends to be a bit more flexible
        (no pun intended), while width tends to be
        more rigid, but it depends on the type 
        of layout you're working with.

        So pick whichever makes more sense to you!

    That's it! We also added background colors below 
    so you can see the boundaries of the column boxes.
*/

#two-columns {
    /* STEP 2 */
    display: flex;
}

#column-1,
#column-2 {
    /* STEP 3, OPTION 1 */
    /* 
    width: 50%;
    */

    /* STEP 3, OPTION 2 */
    flex: 1;
}

#column-1 {
    background-color: lightgreen;
}

#column-2 {
    background-color: #37d37b;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Two Columns - Equal Size (flex)</title>
        <link href="css/basic.css" rel="stylesheet">
    </head>
    <body>
        <div id="two-columns">
            <div id="column-1">
                <h1>Two Columns - Equal Size (flex)</h1>
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
            <div id="column-2">
                <h2>Other Side</h2>
                <p>
                    Generally speaking, don't put text content side-by-side 
                    unless it all fits on the same screen.
                </p>
                <p>
                    For example, a newspaper layout most likely wouldn't
                    work on a web page, because you'd have to scroll down
                    the page and then back up again to read the content,
                    and that's a poor user experience.
                </p>
                <p>
                    Ideally, you'd want to keep the content in each column 
                    equally balanced, to keep it symmetrical, unless you're 
                    going for an asymmetrical design (which can work well 
                    in this kind of layout).
                </p>
            </div>
        </div>
    </body>
</html>
```
