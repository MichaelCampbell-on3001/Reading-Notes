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

Push | | ~pop
     | ----------- | <-top
     |  | 
     |  | 


5. What causes a Stack Overflow? **Answer**

[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘refrence error’? **Answer**
2. What is a ‘syntax error’? **Answer**
3. What is a ‘range error’? **Answer**
4. What is a ‘tyep error’? **Answer**
5. What is a breakpoint? **Answer**
6. What does the word ‘debugger’ do in your code? **Answer**
