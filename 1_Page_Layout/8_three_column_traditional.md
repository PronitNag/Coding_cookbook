```css

* {
box-sizing: border-box;}

body {
margin: 0px;font-family: sans-serif;}


#three-columns {
display: grid;grid-template-columns: 1fr 1fr 1fr;}

#column-1 {
background-color: lightblue;}

#column-2 {
background-color: darkblue;color: white;}

#column-3 {
background-color: aquamarine;}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Three Columns - Traditional (grid)</title>
        <link href="css/basic.css" rel="stylesheet">
    </head>
    <body>
        <div id="three-columns">
            <div id="column-1">
                <h1>Three Columns - Traditional (grid)</h1>
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
            </div>
            <div id="column-2">
                <h3>Lorem ipsum dolor</h3>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                    Porro, commodi similique ipsa tempora perspiciatis, sed 
                    exercitationem reprehenderit sapiente a cumque voluptates 
                    veniam est, quia totam voluptatibus eaque consectetur 
                    optio ipsum.
                </p>
            </div>
            <div id="column-3">
                <h3>Rolod muspi merol</h3>
                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. 
                    Dolore architecto explicabo reprehenderit vel saepe, 
                    illum vitae dicta tempora aperiam repellendus sed 
                    aspernatur corrupti consequatur culpa ratione dolor
                    tempore quas ipsa.
                </p>
            </div>
        </div>
    </body>
</html>
```
