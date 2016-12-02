## Website Performance Optimization portfolio project

To run the page, download the zipfile the start it via index.html

### Optimizations

####index.html

* Adding Cache-control to the Header
* Adding media print to the print.css
* Inline the style.css and the google font (changed URL)
* Resizing and Optimizing Images

####pizza.html



####main.js
function changePizzaSizes was completely rewritten
    ```function changePizzaSizes(size) {
        var newwidth;
        switch (size) {
            case "1":
                newwidth = 25;
            case "2":
                newwidth = 33.3;
            case "3":
                newwidth = 50;
            default:
                console.log("bug in sizeSwitcher");
        }
        //getting the querySelector out of the loop
        var pizzaContainer = document.querySelectorAll(".randomPizzaContainer")
        for (var i = 0; i < pizzaContainer.length; i++) {
            pizzaContainer[i].style.width = newwidth + "%";
        }
    }```


changing the pizza count to 50
```document.addEventListener('DOMContentLoaded', function() {
    var cols = 8;
    var s = 256;
    for (var i = 0; i < 50; i++) {}```

```window.addEventListener('scroll', function () {
   requestAnimationFrame(updatePositions);
});```