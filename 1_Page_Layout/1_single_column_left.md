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

body {
    background-color: #e4f8ff;
}

#navbar {
    background-color: #13135d;
}

#navbar a {
    color: white;
    text-decoration: none;
    display: inline-block;
    padding: 12px 12px 12px 0px;
}

/*
    This is an example of how a single column
    layout aligned to the left might be used.

    This type of layout is not very common 
    anymore, as it typically doesn't make 
    good use of the negative space of wider
    screens.  You may find some blogs or 
    out-dated sites that still use it.

    Note that we share the same column styles
    across multiple containers, both in the 
    navbar and in the main content.

    This is a very common way to prevent page
    content (including navigation) from getting 
    too wide on wider screens and monitors.  
    
    This is generally a good practice, as it
    keeps your viewers' eyes and mouse focused
    on the same part of the screen.

    Also, note that the #navbar-column is found
    inside of the #navbar. It is the #navbar 
    container that's responsible for the dark
    blue background color, but it is the 
    #navbar-column responsible for creating 
    the column in the navbar.
*/

#navbar-column,
.center-column {
    width: 500px;
    padding: 0px 24px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Single Column - Left</title>
        <link href="css/common.css" rel="stylesheet">
    </head>
    <body>
        <div id="navbar">
            <div id="navbar-column">
                <a href="#">BRAND NAME</a>
                <a href="#">LINK 1</a>
                <a href="#">LINK 2</a>
                <a href="#">LINK 3</a>
            </div>
        </div>
        <div class="center-column">
            <h1>Single Column - Left</h1>
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
            <p>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
                Quos sequi, facere ex impedit blanditiis veniam sunt 
                consectetur odio doloremque molestiae deleniti dolores 
                obcaecati consequuntur dolorum? Voluptatem quidem 
                ratione temporibus autem!
            </p>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                Dolorum nemo tenetur quis corporis cumque nostrum 
                temporibus tempora esse? Ullam illo, incidunt veniam quasi 
                quidem expedita animi esse nesciunt minus ab.
            </p>
        </div>
    </body>
</html>
```
