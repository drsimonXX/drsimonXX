#Website Optimization
Website Optimization is a project that showcases performance enhancements made to an existing sample portfolio site. The portfolio site was provided using HTML5, CSS3, Bootstrap, JavaScript and jQuery as a project by [Udacity](http://www.udacity.com "Udacity") as part of its [Front-end nanodegree course](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd001 "Udacity Front-End Nanodegree"). 

##Project Goals
- The goal of the optimizations performed on the main portfolio home page (index.html) is to score a '90' or above using PageSpeed Insights on both mobile and desktop views. 
- The goals of the optimizations performed on Cam's Pizzeria site (pizza.html) are 1) to consistently achieve a frames per second (fps) of '60' while scrolling through the site and 2) to resize the pizzas in less than '5' milliseconds (ms). 

##How To Use the Site
1. In order to view the sample portfolio site with its changes, click [here](https://drsimonxx.github.io/ "Danielle R. Simon's Website Optimization"). *It is preferable that you open the site in Google Chrome so that you can use its Developer Tools*. 
2. Go to [PageSpeed Insights] (https://developers.google.com/speed/pagespeed/insights/ "PageSpeed Insights") and enter in **https://drsimonXX.github.io** in order to measure the mobile and desktop performance. The goal is a score of '90' or above on both views for this page. 
3. Return to the sample portfolio site, scroll down and click on the last link--**"Cam's Pizzeria."** 
4. Open Developer Tools (you can right-click on any white space on the site and select "Inspect") and select "Timeline." 
5. Click the round button/record button and scroll the site in order to measure frames per second (fps), and then press the button again to stop recording. You may need to click on an image of 3 vertically-lined dots, select "More Tools"-->"Rendering Settings"-->"Show FPS Meter" in order to help you view the fps. 
6. Record again, this time while testing the pizza slider. Upon stopping, check how many milliseconds (ms) it took to resize the pizzas.

##Optimizations
- Inlined the CSS in **index.html**
- Inlined the shorter CSS file into **pizza.html**
- Asynchronized JavaScript files in **index.html** and **pizza.html**
- Resized and compressed Cam's profile picture and pizzeria thumbnail in **index.html**
- Resized and compressed pizzeria image in **pizza.html**
- Removed unnecessary styles in Bootstrap CSS file
- Added "media='print'" to print.css style link in **index.html**
- Added media queries to **pizza.html** inline CSS to render site faster on mobile views
- Moved all CSS and JavaScript links to just before closing "body" tag in **index.html** and **pizza.html**
- Changed all instances of "document.querySelector"/"document.querySelectorAll" to "document.getElementById" or "document.getElementByClassName" in **main.js** for pizza.html
- Made the function changePizzaSlices(size) more efficient by adding cases for the size changes and iterating through the pizzas with a 'for' loop in **main.js** for pizza.html
- Applied "transform=translateX()" to the function updatePositions() in **main.js** for pizza.html
- Added "will-change: transform" to the "mover" class in the function updatePositions in the CSS for **pizza.html**
- Removed unnecessary Google font in **index.html**

**For more detailed explanations of changes made in main.js for pizza.html, see the code comments in main.js [here] (https://github.com/drsimonXX/drsimonXX.github.io/blob/master/views/js/main.js "main.js")**.
