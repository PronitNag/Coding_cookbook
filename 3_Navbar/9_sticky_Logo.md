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
#navbar {
    background: linear-gradient(to bottom, green, #3e6d3e);
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0px;
}

#navbar a {
    text-decoration: none;
    color: white;
    padding: 24px;
}

#navbar #logo img {
    width: 150px;
}

#navbar .cta-buttom {
    background-color: white;
    color: green;
    border-radius: 36px;
    padding: 16px 24px;
    font-size: 20px;
    font-weight: bold;
    min-width: 150px;
    text-align: center;
    margin-right: 24px;
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
        <title>Navbar (Header) - Sticky Logo w/ CTA</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="navbar">
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
