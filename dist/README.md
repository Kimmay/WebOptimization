## Website Performance Optimization portfolio project


To run this application: open the file index.html in a web browser.

Optimizations on index.html:
- compressed images
- consolidated CSS files to reduce number of resources needed
- optimized web fonts loading with inline javascript
- inlined above-the-fold CSS for faster rendering
- inlined fetching of CSS file to javascript for faster rendering
- marked google analytics script for async fetching


Optimizations on pizza.html
- compressed images
- added srcset for images to fetch optimally sized image
- optimized pizza resize slider
- optimized background moving pizzas animation

Optimizations on views/js/main.js
resizePizzas():
	- changed pizza size to width % instead of pixel measurement
	- layout call now changes all pizzas to a preset %, instead of measuring current size and adding/subtracting pixels

updatePositions():
	- reduced number of moving pizzas to closer to # you can physically see on screen
	- moved style calculations before all layout calls
	- changed style.left layout call to style.transform for faster rendering
	