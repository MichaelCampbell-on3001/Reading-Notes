# Class 02 Reading Notes 

## State and Props

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? **In the diagram below the render happens first.** ![React Lifecycle Events](https://miro.medium.com/max/1400/0*0saPKFiTUk6W3FYp)
[source](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
2. What is the very first thing to happen in the lifecycle of React? **The constructor method is called before the component is mounted to the DOM.**
3. Put the following things in the order that they happen: **constructor, render, componentWillUnmount,  componentDidMount,  React Updates**
4. What does componentDidMount do? **Allows us to execute the React code when the component is already placed in the DOM**

## [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props? **Anything that can be used to initialize or render you app.**
2. What is the big difference between props and state? **State is handled inside the coompenent and you can update it inside the component, while props are handled outside the component and updated outside the component.**
3. When do we re-render our application? **When you change the state**
4. What are some examples of things that we could store in state? **Input from a user filling out a form can be stored in state.**



