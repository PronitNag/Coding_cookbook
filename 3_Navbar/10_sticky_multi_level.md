```css
/*
    basic page layout setup
*/
* {
    box-sizing: border-box;
}

body {
    margin: 0px;
    font-family: sans-serif;
}

/*
    Navbar setup and configuration
*/
#header {
    position: sticky;
    top: 0px;
}

.content-column {
    width: 800px;
    margin: 0px auto;
}

#navbar-top {
    background: linear-gradient(to bottom, green, #3e6d3e);
}

#navbar-top .content-column {
    display: flex;
    justify-content: space-between;
    align-items: center;
}  

#navbar-top a {
    text-decoration: none;
    color: white;
    padding: 24px 0px;
}

#navbar-top .content-column div a {
    padding: 24px;
}

#navbar-top #logo img {
    width: 150px;
}

#navbar-top .cta-buttom {
    background-color: white;
    color: green;
    border-radius: 36px;
    padding: 16px 24px;
    font-size: 20px;
    font-weight: bold;
    min-width: 150px;
    text-align: center;
}

#navbar-bottom {
    background: linear-gradient(to bottom, yellowgreen, olive);
}

#navbar-bottom .content-column {
    display: flex;
    justify-content: space-between;
}

#navbar-bottom a {
    text-decoration: none;
    color: white;
    padding: 12px 0px;
}

/*
    Layout setup and configuration
*/
#layout {
    width: 600px;
    margin: 48px auto;
    font-size: 24px;
    /* 
        artificially lengthening page to
        enable scrolling to test the 
        sticky navbar
    */
    height: 150vh;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Navbar (Header) - Sticky Multi-Level</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="header">
            <div id="navbar-top">
                <div class="content-column">
                    <a href="#" id="logo">
                        <img src="images/first-logo-hdr.webp" alt="logo">
                    </a>
                    <div>
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                    </div>
                    <a href="#" class="cta-buttom">Sign up</a>
                </div>
            </div>
            <div id="navbar-bottom">
                <div class="content-column">
                    <a href="#">Lower link 1</a>
                    <a href="#">Lower link 2</a>
                    <a href="#">Lower link 3</a>
                    <a href="#">Lower link 4</a>
                    <a href="#">Lower link 5</a>
                </div>
            </div>
        </div>
        <div id="layout">
            <h1>Try scrolling!</h1>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
                Asperiores laborum perspiciatis repellat corporis enim. 
                Asperiores consectetur architecto nobis deleniti 
                blanditiis quisquam in provident perspiciatis non! 
                Et beatae ullam porro voluptatum.
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
                Asperiores laborum perspiciatis repellat corporis enim. 
                Asperiores consectetur architecto nobis deleniti 
                blanditiis quisquam in provident perspiciatis non! 
                Et beatae ullam porro voluptatum.
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
                Asperiores laborum perspiciatis repellat corporis enim. 
                Asperiores consectetur architecto nobis deleniti 
                blanditiis quisquam in provident perspiciatis non! 
                Et beatae ullam porro voluptatum.
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
                Asperiores laborum perspiciatis repellat corporis enim. 
                Asperiores consectetur architecto nobis deleniti 
                blanditiis quisquam in provident perspiciatis non! 
                Et beatae ullam porro voluptatum.
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
                Asperiores laborum perspiciatis repellat corporis enim. 
                Asperiores consectetur architecto nobis deleniti 
                blanditiis quisquam in provident perspiciatis non! 
                Et beatae ullam porro voluptatum.
            </p>
        </div>
    </body>
</html>
```
