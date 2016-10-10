## Website Performance Optimization portfolio project
[View here](https://kaaikman.github.io/frontend-nanodegree-mobile-portfolio/)

### index.html
* Made the js load asynchronously
* Added media to print css link so it only loads on print
* Moved style.css and font loading to bottom of html
  * Inlined font loading based on recommendation of https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery
* Resized/optimized the pizzeria and profilepic images


### main.js
#### -scrolling
* Calculated the value using document.body.scrollTop outside of the for loop in updatePositions()
* Added a smaller image for use as the background pizzas and reduced # of background pizzas
* Replaced document.querySelectorAll with document.getElementsByClassName

#### -resizing
* In changePizzaSizes() moved querySelectorAll out of the for loop
* Got rid of the whole determineDx function and set sizes within the changeSliderLabel cases
