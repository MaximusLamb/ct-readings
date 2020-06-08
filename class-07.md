# Express
## Event driven system
```js
app.get('/thing', (req,res) => {})
```

## The Request Object
```js
(req,..)
/:parameters
app.get('/api/:thing',...) = req.params.thing
```
## Query Strings
```js
http://server/route?ball=round = req.query.ball
```
## The Response Object
```js
(..., res)
```
* Responsible for sending data back to the browser
* Has methods like send() and status() that Express uses to format the output to the browser properly
* Sends Headers
* Cookies
* Status Codes
* Express Middleware
### What does it do?
* A series of functions that the request “goes through”
* Each function receives request, response and next as parameters
## Types of middleware
* Application and Route
### Application
* Error Handling
* Bringing in other routes
* Applies Defaults
* JSON, Body and Form Parsing
* Runs on every request
### Route
* Dealing with specific things for a route
* Generally, things many routes would participate in
* Are you logged in?
* What is your IP?
* Have we seen you here before?
* How can we take advantage?
Logging
* Dynamic Model Loading
* Browser, Location, User specific content
* Consistent Data Transition/Modeling/Preparation (Pre-Render)
* Modularization & Separation of Concerns
* Modularizing your code into logical chunks

## CRUD Operations with REST and Express
### CREATE
* app.post('/resource')
## READ
* app.get('/resource')
## UPDATE
* app.put('/resource/:id')
## DESTROY
* app.get('/resource/:id')
