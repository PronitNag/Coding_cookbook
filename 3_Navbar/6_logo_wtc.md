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
    align-items: center;
}

#navbar a {
    text-decoration: none;
    color: white;
    padding: 24px;
}

#navbar #logo {
    margin-right: auto;
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
```
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Navbar (Header) - Logo w/ CTA</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="navbar">
            <a href="#" id="logo">
                <img src="images/first-logo-hdr.webp" alt="logo">
            </a>
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
            <a href="#" class="cta-buttom">Sign up</a>
        </div>
    </body>
</html>
```
