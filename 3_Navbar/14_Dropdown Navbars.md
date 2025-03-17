```css
/*
    General Page Layout styling *********************************
*/

* {
    box-sizing: border-box;
}

body {
    margin: 0px;
    font-family: sans-serif;
}

/*
    Navbar styling **********************************************
*/
#navbar {
    background: linear-gradient(to bottom, #109cb8, #0e5b96);
    display: flex;
    align-items: center;
}

#navbar a {
    display: inline-block;
    text-decoration: none;
    color: white;
    padding: 24px;
}

#navbar a:hover {
    background: linear-gradient(to top, #109cb8, #0e5b96);
}

#navbar #logo {
    margin-right: auto;
    font-weight: bold;
    font-size: 36px;
    padding-top: 13px;
    padding-bottom: 12px;
}

/*
    Dropdown styling ********************************************
*/
.dropdown-container {
    position: relative;
}

.dropdown-menu {
    position: absolute;
    opacity: 0;
    visibility: hidden;
    transition: 
        opacity 0.25s,
        visibility 0.25s;

    /*
        If your dropdown menu seems to be placed
        behind content on your page, you may need
        to include a z-index, which pull it 
        closer to you as a viewer.
    */
    z-index: 10;
}

/*
    This selector targets dropdown-containers
    that are the last child of their parent,
    and looks inside of them for a dropdown-menu.

    If found, we target it and anchor it
    to the right of its parent container
*/
.dropdown-container:last-child .dropdown-menu {
    right: 0px;
}

/*
    This is the selector responsible for
    revealing the dropdown menu.

    Note that the :hover pseudo-class is 
    attached to the CONTAINER, not the MENU.

    We can't hover over the menu when it's
    hidden; we only want it to display when
    the trigger link in the container is 
    hovered over.
*/
.dropdown-container:hover .dropdown-menu {
    opacity: 1;
    visibility: visible;
}

.dropdown-menu a {
    background-color: darkslateblue;
    width: 100%;
    min-width: 200px;
}

/*
    We need to be a bit more specific with
    our selectors in order to override the
    anchor hover state we declared earlier.

    To do so, we need to include both
    #navbar and .dropdown-menu.

    Also note, using background-color
    won't work, because in our original
    anchor hover, we used the background
    property to set a linear-gradient().

    So, to override it, we need to use
    the same shorthand background property.
*/
#navbar .dropdown-menu a:hover {
    background: slateblue;
}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Dropdown Navbars (Demo)</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css" integrity="sha512-xh6O/CkQoPOWDdYTDqeRdPCVd1SpvCA9XXcUnZS2FmJNp1coAFzvtCN9BmamE+4aHK8yyUHUSCcJHgXloTyT2A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
        <link href="css/style.css" rel="stylesheet" data-meal-prep>
    </head>
    <body>
        <div id="navbar">
            <a id="logo" href="#">BRAND NAME</a>

            <!-- First Dropdown -->
            <div class="dropdown-container">
                <a href="#">Gallery <i class="fa-solid fa-chevron-down"></i></a>
                <div class="dropdown-menu">
                    <a href="#">Drawings</a>
                    <a href="#">Photography</a>
                    <a href="#">Photoshop</a>
                    <a href="#">Illustrator</a>
                </div>
            </div>

            <!-- Second Dropdown -->
            <div class="dropdown-container">
                <!-- ...and here... -->
                <a href="#">About <i class="fa-solid fa-chevron-down"></i></a>
                <div class="dropdown-menu">
                    <a href="#">Passions</a>
                    <a href="#">Hobbies</a>
                    <a href="#">Goals</a>
                </div>
            </div>

            <a href="#">Contact</a>

            <!-- Third Dropdown -->
            <div class="dropdown-container">
                <!-- ...and here -->
                <a href="#">More <i class="fa-solid fa-chevron-down"></i></a>
                <div class="dropdown-menu">
                    <a href="#">Collaborations</a>
                    <a href="#">Commissions</a>
                    <a href="#">Pricing</a>
                </div>
            </div>
        </div>
    </body>
</html>
```
