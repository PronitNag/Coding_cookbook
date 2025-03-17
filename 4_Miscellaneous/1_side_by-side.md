```css
* {
    box-sizing: border-box;
}
body {
    margin: 0px;
    font-family: sans-serif;
}
img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

#nav {
    background-color: #fff0cb;
    padding: 20px;
    /*
        display: flex; is required to turn an element 
        into a flexbox container; this will force 
        elements inside the container to be side by side 
        by default.
    */
    display: flex;
    justify-content: center;
    gap: 125px;
}

#nav a {
    color: black;
    text-decoration: none;
    font-weight: bold;
}

#flex-side-by-side {
    width: 80vw;
    max-width: 800px;
    margin: 40px auto;
    display: flex;
    align-items: center;
    gap: 50px;
}

.image-container {
    height: 400px;
}

#grid-side-by-side {
    background-color: #fff0cb;
    padding: 40px;
    /*
        display: grid; is required to turn an element 
        into a CSS Grid container; however, there is 
        another step that must be taken before you get 
        the grid items side by side:

        The grid-template-columns property is required 
        to get things side by side in a grid; you'll need
        to specify the width of each column before your
        content will shift side by side.
    */
    display: grid;
    grid-template-columns: 250px 250px;
    grid-auto-rows: 150px;
    justify-content: center;
    gap: 50px;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Side-by-Side with Responsiveness</title>
        <link href="css/page0.css" rel="stylesheet">
    </head>
    <body>
        <!-- Navigation with Flexbox -->
        <div id="nav">
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
        </div>

        <!-- Flexbox Side-by-side -->
        <div id="flex-side-by-side">
            <div class="image-container">
                <img src="images/photo-1.jpg" alt="photo">
            </div>
            <div class="content">
                <h1>Flexbox Side-by-Side Responsiveness</h1>
                <p>Lorem, ipsum dolor sit amet consectetur</p>
            </div>
        </div>

        <!-- Grid Side-by-side -->
        <div id="grid-side-by-side">
            <img src="images/photo-2.jpg" alt="photo">
            <img src="images/photo-3.jpg" alt="photo">
            <img src="images/photo-4.jpg" alt="photo">
            <img src="images/photo-5.jpg" alt="photo">
        </div>
    </body>
</html>
```

