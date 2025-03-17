```css

* {
box-sizing: border-box;}

body {
margin: 0px;font-family: sans-serif;}


body {
background-color: #E0E0E0;color: #111111;}

#outer-layout {
display: grid;grid-template-columns: 1fr 800px 1fr;grid-template-areas: ". content-area .";}

#inner-layout {
grid-area: content-area;display: flex;}


#column-1 {
background-color: white;padding: 0px 12px;flex: 2;}

#column-2 {
background-color: white;padding: 0px 12px;flex: 1;}

#column-3 {
background-color: white;padding: 0px 12px;flex: 1;}

#inner-layout img {
margin-top: 24px;width: 100%;}

#inner-layout h2,
#inner-layout h3 {
border-bottom: 2px solid #888888;padding-bottom: 4px;margin-bottom: 0px;}

#inner-layout p {
margin-top: 12px;}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Mixed Columns (grid + flex)</title>
        <link href="css/mixed.css" rel="stylesheet">
    </head>
    <body>
        <div id="outer-layout">
            <div id="inner-layout">
                <div id="column-1">
                    <img 
                        src="images/flexible-seal.jpg"
                        alt="flexible seal steals the show at beach yoga event"
                    >
                    <h2>
                        Flexible Seal Steals the Show at Beach Yoga Event On Sunday
                    </h2>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                        Porro, commodi similique ipsa tempora perspiciatis, sed 
                        exercitationem reprehenderit sapiente a cumque voluptates 
                        veniam est, quia totam voluptatibus eaque consectetur 
                        optio ipsum.
                    </p>
                    <h3>Ipsum dolor lorem</h3>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
                        Porro, commodi similique ipsa tempora perspiciatis, sed 
                        exercitationem reprehenderit sapiente a cumque voluptates 
                        veniam est, quia totam voluptatibus eaque consectetur 
                        optio ipsum.
                    </p>
                </div>
                <div id="column-2">
                    <h3>Mixed Columns use both grid and flex</h3>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Cupiditate necessitatibus ab ipsum? Natus suscipit 
                        asperiores alias ipsam, cum, accusamus quisquam nam 
                        magnam aspernatur vel tenetur quibusdam. Consequatur 
                        itaque similique provident. 
                    </p>
                    <p>
                        Lorem ipsum dolor sit, amet 
                        consectetur adipisicing elit. Iste ipsum veritatis ullam, 
                        dolor tempora quo. Omnis, id pariatur. Accusantium facere 
                        quo praesentium aspernatur omnis qui ratione impedit 
                        aperiam minima dolorem. Consequatur culpa ratione dolor
                        tempore quas ipsa tempora perspiciatis.
                    </p>
                </div>
                <div id="column-3">
                    <h3>Rolod muspi merol rutetcesnoc</h3>
                    <p>
                        Lorem ipsum dolor sit amet consectetur, adipisicing elit. 
                        Dolore architecto explicabo reprehenderit vel saepe, 
                        illum vitae dicta tempora aperiam repellendus sed 
                        aspernatur corrupti consequatur culpa ratione dolor
                        tempore quas ipsa.
                    </p>
                    <h3>Merol muspi</h3>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        Soluta hic qui facilis sequi, repellendus voluptates 
                        sunt sed aliquam? Tempore explicabo necessitatibus 
                        libero aut, minima error ratione iste consequuntur 
                        molestiae doloremque!
                    </p>
                </div>
            </div>
        </div>
    </body>
</html
```
