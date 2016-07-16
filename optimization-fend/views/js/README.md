To run, simply go to https://amansn.github.io/optimization-fend/views/pizza.html?#randomPizzas

in your web browser.

How did I optimize main.js?

1. In the updatedPositions function, I changed querySelectorAll to getElementsByClassName.
2. In the same function, I moved the initial part of the equation outisde the for loop.
3. In the changePizzaSizes function, I moved the variables dx and newwidth outside the for loop to avoid looping.
4. In the event listener for DOMContentLoaded, I changed the number of pizzas from 200 to 25 because only a handful are showing. 200 was too much.
5. I resized the pizzeria image because an image that large was unnecessary to load up. This lowered the bytes that needed to be downloaded in the Critical Rendering Path.
