# Passing Functions as Props

1. What does .map() return? **It returns the original array, until you specify a change for example : `.map((number) => number * 2)`. In this case the `.map()` function takes in an array of numbers and doubles their values**
4. If I want to loop through an array and display each value in JSX, how do I do that in React? **We can loop through the numbers array using the JavaScript map() function, then return a `<li>` element for each item. We can then assign the resulting array of elements to listItems. After that, you can wrap your list in an `<ul>` and render to the DOM or make it into a new component.**
5. Each list item needs a unique **Key**. 
6. What is the purpose of a key? **React relies on Keys to identify which items have changed, added, or removed. Keys provide stable identity to elements inside an array.**


