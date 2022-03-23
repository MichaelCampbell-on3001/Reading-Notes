# Node Ecosystem, TDD, CI/CD

1. Describe (in plain English) what Array.map() does: **Array.map( ) itirates over an array and return the array with a new specified format.**

1. Describe (in plain English) what Array.reduce() does **Similar to .map .reduce iterates over an element aand provide a callback function or "Accumulator". You can set the values on the accumulator to give it a custom starting positiion. A cycle is complete when it returns the final accumulator value.**

1. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
 - **With normal Promise .then() syntax**

        ` request
        .post('/api/pet')
        .send({ name: 'Manny', species: 'cat' })
        .set('X-API-Key', 'foobar')
        .set('Accept', 'application/json')
       .then(res => {
       alert('yay got ' + JSON.stringify(res.body));
       });` 
    
    [Attribution for above solution](https://visionmedia.github.io/superagent/)

 - **Again with async / await syntax:**

        `async function AsyncFunction() {
        let API = await superagent.get('URL-API');
        console.log(API.body);
        } AsyncFunction();`

1. Explain promises as though you were mentoring a Code 301 level student:
In programming, a **promise** is a program calls a function expecting that it will do some useful thing and return the result which the calling program can use. 
The outcome of calling the functions, no matter whether they pass or fail, and any associated data is a **PROMISE**.

1. Are all callback functions considered to be Asynchronous? Why or Why Not?
- Asyncinous callbacks are specific to arguments when a function is called
-  Callbacks are not asynchronous by nature, but can be used for asynchronous purposes.
- I suppose any function can become a callback function if it is passed as an argument.
- JS callbacks are only asynchronous if they rely on an API 
