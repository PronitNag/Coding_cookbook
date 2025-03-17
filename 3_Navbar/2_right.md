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
    justify-content: flex-end;
}

#navbar a {
    text-decoration: none;
    color: white;
    padding: 24px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Navbar (Header) - Right</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="navbar">
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
            <a href="#">Link 4</a>
        </div>
    </body>
</html>
```
