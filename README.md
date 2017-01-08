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

### To run the application

1. Download the /dist/ folder in your computer.
1. To inspect the site on your phone, you can run a local server:

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080.
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely:

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights and Chrome DevTools!