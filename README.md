## Website Performance Optimization portfolio project

To run the app, download entire directory and open `index.html` in a browser.

### Part 1: Optimize PageSpeed Insights score for index.html

1. Optimize images using grunt responsive_images and editing image src links.

2. Move external CSS files into index.html header.

3. Async javascript links in header.

4. Setup web font loader to prevent render blocking by font load.

PageSpeed Insights score: **94/100**

### Part 2: Optimize Frames per Second in pizza.html

**Scrolling**

- reduced nummber of pizzas loaded
- document.getElementById() and document.getElementsByClassName()
- DOM calls mover outside of for loops and saved to local variable
- Saved array lengths in local variable
- Declare variables outside of loops


### Provided information

####Part 1: Optimize PageSpeed Insights score for index.html

    ** Inline css recommended by PageSpeed in order to get more speed
    ** Took out the font link, too heavy for the loading process.
    ** CSS for media print was made.
    ** Asyncronimous call for perfmatters.js and Google analytics.js
    ** All images were optimized using http://optimizilla.com/


####Part 2: Optimize Frames per Second in pizza.html
    ** CSS files were minimized for better loading process.
    ** To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. You will find instructive comments in main.js.
    ** Resizes pizza function was optimized including the width selector within it's code for better performance.  Also using a % value for resizing.
    ** Replaced the call for the document pizza container in order to use it within the for loop
    ** Update position function optimized:  properties obtained by using getElementsByClassName.  Stored length of the object 'mover' and also the scrollTop propertie of the Document.
    ** Variable 'phase' declared outside the loop.
    ** The 'DOMContentLoaded' even listener optimized: variables declare outside the loop, number of pizzas to generate obtain outside the loop (tried with window.screen.height propertie but it didn't work well).
    ** CSS files minimized.



    note: Browser caching, configured server-side, could have reduced page loading time.