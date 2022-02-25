# In memory storage

[Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a ‘call’? **function invocation**
2. How many ‘calls’ can happen at once? **one at a time**
3. What does LIFO mean? **Last In, First Out**
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

`function firstFunction(){
  throw new Error('Stack Trace Error');
}`

`function secondFunction(){
  firstFunction();
}`

`function thirdFunction(){
  secondFunction();
}`

`thirdFunction();`
 |push  | 
 | ----------- | 
 | Pop | 
 | Top  | 
 | |
 | |
 | |
 | |


5. What causes a Stack Overflow? ** When there is a a function that calls itself without an exit point**

[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘refrence error’? **An error that is returned when you try to use a variable that is not yet declared you get this type os errors.**
2. What is a ‘syntax error’? **When something that cannot be parsed in terms of syntax, like trying to parse an invalid object using JSON.parse.**
3. What is a ‘range error’? **Try to manipulate an object with some kind of length and give it an invalid length.**
4. What is a ‘type error’? **When accessing a property in an undefined type of variable**
5. What is a breakpoint? **A breakpoint can be achieved by putting a debugger statement in your code in the line you want to break.**
6. What does the word ‘debugger’ do in your code? **break it**
