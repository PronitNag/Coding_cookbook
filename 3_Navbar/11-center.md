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
    Footer setup and configuration
*/
#footer {
    background: linear-gradient(to bottom, teal, #01482e);
    color: white;
    padding: 12px;
}

#footer a {
    text-decoration: none;
    color: white;
}

#footer-navbar {
    width: 800px;
    margin: 0px auto;
    display: flex;
    justify-content: space-between;
}

/*
    Layout setup and configuration
*/
#layout {
    width: 800px;
    margin: 48px auto;
    font-size: 24px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Navbar (Footer) - Center</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="layout">
            <h1>Lorem ipsum dolor</h1>
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
        <div id="footer">
            <div id="footer-navbar">
                <span>&copy; FIRST 2023</span>
                <a href="#">Footer Link 1</a>
                <a href="#">Footer Link 2</a>
                <a href="#">Footer Link 3</a>
                <a href="#">Footer Link 4</a>
            </div>
        </div>
    </body>
</html>
```
