# Passing Functions as Props

1. What does .map() return? **It returns the original array, until you specify a change for example : `.map((number) => number * 2)`. In this case the `.map()` function takes in an array of numbers and doubles their values**
4. If I want to loop through an array and display each value in JSX, how do I do that in React? **We can loop through the numbers array using the JavaScript map() function, then return a `<li>` element for each item. We can then assign the resulting array of elements to listItems. After that, you can wrap your list in an `<ul>` and render to the DOM or make it into a new component.**
5. Each list item needs a unique **Key**. 
6. What is the purpose of a key? **React relies on Keys to identify which items have changed, added, or removed. Keys provide stable identity to elements inside an array.**

[Source](https://reactjs.org/docs/lists-and-keys.html)

# The Spread Operator

1. What is the spread operator? **It refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments. It is also quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.**
2. List 4 things that the spread operator can do.**1. Using an array as arguments 2. Adding to state in React 3.Combining objects 4.Converting NodeList to an array**
3. Give an example of using the spread operator to combine two arrays. **You can use array concatenation. ex:** 

**`const myArray = [`🤪`,`🐻`,`🎌`]`**

**`const yourArray = [`🙂`,`🤗`,`🤩`]`**

**`const ourArray = [...myArray,...yourArray]`**

**`console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩`**
[source](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

4. Give an example of using the spread operator to add a new item to an array.**The syntax to add a new item to an array is to  use to syntax `(...)`. 
For example:**

**`const mybox =[my stuff]`**

**`const yourbox =[your stuff...my stuff] `**
**Once you `console.log` it you'll discover "my stuff" and "your stuff" can now be found in "your box".**

6. Give an example of using the spread operator to combine two objects into one.**The Spread syntax can be used for combining the properties and methods on objects into a new object. For example:**
**`const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}`**

# How to Pass Functions Between Components
[Source](https://www.youtube.com/watch?v=c05OL7XbwXU)
1. In the video, what is the first step that the developer does to pass functions between components? **The dev created the function and mapped over the array.**
2. In your own words, what does the increment function do? **The increment function allows you to search through an array and increase the counter when it finds what you are searching for.**
3. How can you pass a method from a parent component into a child component? **You can pass it in like any other props**
4. How does the child component invoke a method that was passed to it from a parent component? **The child passes whatever it was givien back to the increment method above.**


