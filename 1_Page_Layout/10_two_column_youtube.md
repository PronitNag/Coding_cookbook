```css
* {
box-sizing: border-box;}

body {
margin: 0px;font-family: sans-serif;}

#grid-layout {
display: grid;grid-template-columns: 250px 1fr;grid-template-areas: "header header""sidebar main";}

#header {
grid-area: header;padding: 0px 36px;}

#sidebar {
grid-area: sidebar;padding: 0px 24px;}

#main {
grid-area: main;display: flex;flex-wrap: wrap;}

#header a {
text-decoration: none;}

#header #me {
color: #111111;}

#header #tube {
color: white;background-color: red;padding: 4px;border-radius: 12px;}

#sidebar ul {
padding: 12px 0px;margin: 0px;list-style-type: none;border-bottom: 1px solid #AAAAAA}


#sidebar ul a {
text-decoration: none;color: #111111;display: block;padding: 12px;}

#sidebar ul a:hover {
background-color: #EEEEEE;border-radius: 12px;}

.metube-item {
flex: 250px;margin-right: 12px;margin-bottom: 24px;}

.metube-item .thumbnail-placeholder {
aspect-ratio: 16 /9;background: radial-gradient(at top left, crimson, orange);border-radius: 8px;}


.metube-item h4 {
margin: 8px;}


.metube-item h4 a {
text-decoration: none;color: #111111;display: block;}


.metube-item h4 a:hover {
text-decoration: underline;}


.metube-item .video-details {
margin: 8px;font-size: 14px;}


.metube-item .video-channel {
margin-bottom: 4px;}
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Two Columns - YouTube Look-alike (grid + flex)</title>
        <link href="css/page9.css" rel="stylesheet">
    </head>
    <body>
        <div id="grid-layout">
            <div id="header">
                <h1>
                    <a href="#">
                        <span id="me">Me</span><span id="tube">Tube</span>
                    </a>
                </h1>
            </div>
            <div id="sidebar">
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Shorts</a></li>
                    <li><a href="#">Subscriptions</a></li>
                </ul>
                <ul>
                    <li><a href="#">Library</a></li>
                    <li><a href="#">History</a></li>
                    <li><a href="#">Your videos</a></li>
                    <li><a href="#">Your movies & TV</a></li>
                    <li><a href="#">Watch Later</a></li>
                </ul>
            </div>
            <div id="main">
                <div class="metube-item">
                    <div class="thumbnail-placeholder"></div>
                    <h4><a href="#">MeTube Video Title</a></h4>
                    <div class="video-details">
                        <div class="video-channel">Channel Placeholder</div>
                        <div class="views-and-post">
                            <span class="video-views">1.9K views</span>
                            &bull; 
                            <span class="video-post">8 hours ago</span>
                        </div>
                    </div>
                </div>
                <div class="metube-item">
                    <div class="thumbnail-placeholder"></div>
                    <h4><a href="#">MeTube Video Title</a></h4>
                    <div class="video-details">
                        <div class="video-channel">Channel Placeholder</div>
                        <div class="views-and-post">
                            <span class="video-views">1.9K views</span>
                            &bull; 
                            <span class="video-post">8 hours ago</span>
                        </div>
                    </div>
                </div>
                <div class="metube-item">
                    <div class="thumbnail-placeholder"></div>
                    <h4><a href="#">MeTube Video Title</a></h4>
                    <div class="video-details">
                        <div class="video-channel">Channel Placeholder</div>
                        <div class="views-and-post">
                            <span class="video-views">1.9K views</span>
                            &bull; 
                            <span class="video-post">8 hours ago</span>
                        </div>
                    </div>
                </div>
                <div class="metube-item">
                    <div class="thumbnail-placeholder"></div>
                    <h4><a href="#">MeTube Video Title</a></h4>
                    <div class="video-details">
                        <div class="video-channel">Channel Placeholder</div>
                        <div class="views-and-post">
                            <span class="video-views">1.9K views</span>
                            &bull; 
                            <span class="video-post">8 hours ago</span>
                        </div>
                    </div>
                </div>
                <div class="metube-item">
                    <div class="thumbnail-placeholder"></div>
                    <h4><a href="#">MeTube Video Title</a></h4>
                    <div class="video-details">
                        <div class="video-channel">Channel Placeholder</div>
                        <div class="views-and-post">
                            <span class="video-views">1.9K views</span>
                            &bull; 
                            <span class="video-post">8 hours ago</span>
                        </div>
                    </div>
                </div>
                <div class="metube-item">
                    <div class="thumbnail-placeholder"></div>
                    <h4><a href="#">MeTube Video Title</a></h4>
                    <div class="video-details">
                        <div class="video-channel">Channel Placeholder</div>
                        <div class="views-and-post">
                            <span class="video-views">1.9K views</span>
                            &bull; 
                            <span class="video-post">8 hours ago</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
```
