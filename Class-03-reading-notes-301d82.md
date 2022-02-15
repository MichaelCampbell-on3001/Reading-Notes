# Passing Functions as Props

1. What does .map() return? **It returns the original array, until you specify a change for example : `.map((number) => number * 2)`. In this case the `.map()` function takes in an array of numbers and doubles their values**
4. If I want to loop through an array and display each value in JSX, how do I do that in React? **We can loop through the numbers array using the JavaScript map() function, then return a `<li>` element for each item. We can then assign the resulting array of elements to listItems. After that, you can wrap your list in an `<ul>` and render to the DOM or make it into a new component.**
5. Each list item needs a unique **Key**. 
6. What is the purpose of a key? **React relies on Keys to identify which items have changed, added, or removed. Keys provide stable identity to elements inside an array.**

[Source](https://reactjs.org/docs/lists-and-keys.html)

# The Spread Operator

1. What is the spread operator? **It refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments. It is also quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.**
2. List 4 things that the spread operator can do.**1. Using an array as arguments 2. Adding to state in React 3.Combining objects 4.Converting NodeList to an array**
3. Give an example of using the spread operator to combine two arrays.**You can use array concatenation. ex: 
`const myArray = [`🤪`,`🐻`,`🎌`]

const yourArray = [`🙂`,`🤗`,`🤩`]

const ourArray = [...myArray,...yourArray]

console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩`**

4. Give an example of using the spread operator to add a new item to an array.**Answer**
5. Give an example of using the spread operator to combine two objects into one.**Answer**
[source](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
