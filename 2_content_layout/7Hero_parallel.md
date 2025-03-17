```css
* {
    box-sizing: border-box
}

body {
    margin: 0px;
    font-family: sans-serif;
}

#hero-5 {
    background-image: url("../images/desert-tumbleweed.jpg");
    height: 100vh;
    background-size: cover;
    background-position: center center;
    background-attachment: fixed;
    position: relative;
    margin-bottom: 100px;
}

#hero-5 .hero-content {
    text-align: right;
    position: absolute;
    top: 5%;
    right: 10%;
}

#hero-5 h2 {
    font-size: 120px;
    margin-bottom: 60px;
}

#hero-5 h4 {
    font-size: 48px;
}

/* filler section, unrelated to the hero styling */
#main {
    height: 100vh;
}

h1 {
    font-size: 36px;
}

p {
    font-size: 20px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Hero - Parallax (position)</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="hero-5">
            <div class="hero-content">
                <h2>Sigh...</h2>
                <h4>Some days be like this</h4>
            </div>
        </div>

        <!-- Filler section, unrelated to hero content or structure -->
        <div id="main">
            <h1>This is simply filler text...</h1>
            <p>
                ...so you can see how the parallax hero behaves as you
                scroll down the page.
            </p>
            <p>
                Lorem ipsum dolor, sit amet consectetur adipisicing 
                elit. Debitis illo adipisci distinctio inventore 
                asperiores sit, suscipit neque dignissimos doloribus 
                fuga similique in enim possimus voluptas facere qui, 
                aspernatur a quidem?
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing 
                elit. Debitis explicabo eum quod voluptas eaque quas? 
                Culpa aliquid, sequi commodi adipisci eaque sapiente. 
                Animi eius voluptate odio ipsum similique nemo 
                officiis!
            </p>
            <p>
                Lorem ipsum dolor, sit amet consectetur adipisicing 
                elit. Debitis illo adipisci distinctio inventore 
                asperiores sit, suscipit neque dignissimos doloribus 
                fuga similique in enim possimus voluptas facere qui, 
                aspernatur a quidem?
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing 
                elit. Debitis explicabo eum quod voluptas eaque quas? 
                Culpa aliquid, sequi commodi adipisci eaque sapiente. 
                Animi eius voluptate odio ipsum similique nemo 
                officiis!
            </p>
        </div>
    </body>
</html>
```
