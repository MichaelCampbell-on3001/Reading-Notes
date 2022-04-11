# Day 5 Reading Notes

## [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the single responsibility principle and how does it apply to components? **A component should only do one thing, but if it ends up growing, it should be broken up into smaller subcomponents.**
2. What does it mean to build a ‘static’ version of your application? **A static version of your app is one that has the data, but no interactivity.**
3. Once you have a static application, what do you need to add? **Your data**
4. What are the three questions you can ask to determine if something is state? **Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.
** [^1]
5. How can you identify where state needs to live?
**A checklist to determine how to identify where state needs to be:**
 - [ ] Identify every component that renders something based on that state.
- [ ] Find a common owner component (a single component above all the components that need the state in the hierarchy).
- [ ] Either the common owner or another component higher up in the hierarchy should own the state.
- [ ] If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”? **Higher order functions are functions that operate on other functions, either by taking them as arguments or by returning them.**
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing? **`return m => m > n;` isreturning the greater value.**
3. Explain how either map or reduce operates, with regards to higher-order functions. **You can use map to go over functions and return an array of thoses functions listed by name, while Reduce can be used to find the function with the longest script.**

[^1]: [Source](https://reactjs.org/docs/thinking-in-react.html)
