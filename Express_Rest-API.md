# Class 3 Exoress Rest API

## [Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

### **Classes** 

- Classes are templates for creating objects.  

### **Class Declarations**
- Can be considered "special functions" 
- Syntax has two components: **class expression** and **class declarations**.

### **Class Expressions**
- Another way to define a class
- Can be named or unnamed
- Named class expression is local to the class's body
- Can be accessed via the name property

### **Class Body Methods**
 The body of a class is the part that is in curly brackets {}. This is where you define class members, such as methods or constructor.

### **Strict mode**
- Code written in strict mode is subject to stricter syntax

### **Constructor**

- A special method for creating an object. 
- Only be one special method with the name "constructor"
- can use the super keyword to call the constructor of the super clas

### **Static initialization blocks**
- Allows flexible initialization of class static properties 
- all static items are evaluated in declaration order

### **[Prototype methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Method_definitions)**

### **[Generator methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Iterators_and_Generators)**

### **Static methods and properties**
- Defines a static method or property for a class.
-  Called without instantiating their class.
- Cannot be called through a class instance.
- Used to create utility functions.



## [Using Express Routing](https://expressjs.com/en/guide/routing.html)

### **Routing** - *how an application’s endpoints (URIs) respond to client requests*

### **Route methods**

- A product of one of the HTTP methods, and is attached to an to the express class.
- Supports methods that correspond to all HTTP request methods (GET, POST, PUT, DELETE)
- **App.all()**, used to load middleware functions at a path for **all** HTTP request methods.

### **Route paths**

This route path will match requests to the root route, /.

`app.get('/', (req, res) => {
  res.send('root')
})`

This route path will match requests to /about.

`app.get('/about', (req, res) => {
  res.send('about')
})`

[more here](https://expressjs.com/en/guide/routing.html)

### **Route parameters**
- URL segments that are used to capture the values in the URL.
- They are then populated in the req.params object.
- The route parameter specified in the path is the key.

### **Route handlers**
-  Can be in the form of a function, an array of functions, or combinations of both.
An example of a callback function handling a route:

`app.get('/example/a', (req, res) => {
  res.send('Hello from A!')
})`

### **Response methods**
- Can send a response to the client, and terminate the request-response cycle.
- Don't leave the client hanging, call a method.

### **app.route()**
- Used to create create chainable route handlers.
- Helps reduce redundancy and typos.

### **express.Router**
- Creates modular, mountable route handlers.
- Often referred to as a “mini-app”.
- 



## [Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

This article goes through step by step to use the Router in ExpressJS4.0

**Below are the Routes expected if you follow the tutorial.**

`...

    // ROUTES
    // ==============================================

    app.route('/login')

        // show the form (GET http://localhost:8080/login)
        .get(function(req, res) {
            res.send('this is the login form');
        })

        // process the form (POST http://localhost:8080/login)
        .post(function(req, res) {
            console.log('processing');
            res.send('processing the login form!');
        });

    ...`
