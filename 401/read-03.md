# Express REST API
- Name 3 real world use cases where you’d want to change the request with custom middleware
  - Authentication and token assignment
  - Capturing request data like time (ms), route, and IP
  - Translation [ref:](https://www.freecodecamp.org/news/what-is-middleware-with-example-use-cases/) 

### True or false: The route handler is middleware?

- Yes? and No? - I seems like you can build routes as middleware, but it seems more likely that you might modify a route hit. Routes also dont tend to have the "next" param which from lecture sounds like THE pre-requisite for being considered middleware

### In what ways can a middleware function end the process and send data to the browser?
- calling or returning 'next(err)' with an error will end the process and give the error to the user. there is also manual ways to end the operation like '.end()'.
[ref:](https://www.geeksforgeeks.org/express-js-res-end-function/)

### At what point in the request lifecycle can you “inject” middleware?
- While its refered to as happening in the middle of the request it actually occurs before its sent off but after the user input

### What can cause express to error with “Request headers sent twice, cannot start a second response”
- when two functions get called that both generate header data for the responese

## Vocabulary Terms
- Middleware - is that makes changes to info going between client and server or between any two entities in the WRRC.
- Request Object - The package of data coming from the 'client'
- Response Object - Where data lives on its way back to the 'client'
- Application Middleware - "Bind application-level middleware to an instance of the app object by using the app.use() and app.METHOD() functions, where METHOD is the HTTP method of the request that the middleware function handles (such as GET, PUT, or POST) in lowercase." [ref:](http://expressjs.com/en/guide/using-middleware.html#middleware.application)
- Routing Middleware - "Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router()."[ref:](http://expressjs.com/en/guide/using-middleware.html#middleware.application)
- Test Driven Development - TDD where the app spcifications determine the testing components first then the app is build to satisfy these tests.
- Behavioral Testing - "is a branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests. Like Domain Driven Design (DDD), an early step in BDD is the definition of a shared vocabulary between stakeholders, domain experts, and engineers."[ref:](https://medium.com/javascript-scene/behavior-driven-development-bdd-and-functional-testing-62084ad7f1f2)

## Preview

Which 3 things had you heard about previously and now have better clarity on?
- I had heard of middleware is some tutorials I had watched prior.
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- I hoping to better solidify the last 3 things we learned in lecture/demo. :)
What are you most excited about trying to implement or see how it works?
- I really like the real time information feedback you can get from middleware.