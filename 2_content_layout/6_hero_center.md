```css
* {
    box-sizing: border-box
}

body {
    margin: 0px;
    font-family: sans-serif;
}

#hero-3 {
    background-image: url("../images/orange-wildflowers.jpg");
    height: 100vh;
    background-size: cover;
    background-position: center center;
    position: relative;
    margin-bottom: 100px;
}

#hero-3 .hero-content {
    position: absolute;
    top: 10%;
    left: 15%;
}

#hero-3 h2 {
    font-size: 72px;
    margin-bottom: 36px;
}

#hero-3 h4 {
    font-size: 24px;
    margin: 0px;
}

#hero-3 a {
    font-size: 14px;
    display: inline-block;
    background-color: #333333;
    color: white;
    text-decoration: none;
    padding: 24px;
    margin-top: 36px;
    margin-right: 24px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Hero - Left (position)</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="hero-3">
            <div class="hero-content">
                <h2>Relax</h2>
                <h4>Take a deep breath</h4>
                <div>
                    <a href="#">BREATHE IN</a>
                    <a href="#">BREATHE OUT</a>
                </div>
            </div>
        </div>
    </body>
</html>
```
