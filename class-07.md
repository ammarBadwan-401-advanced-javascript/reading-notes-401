# Express

## Express Routing

* Event driven system:

`app.get('/thing', (req,res) => {})` , this is the same pattern in Vanilla JS and jQuery, it activates when an event happens on "/thing/", this function runs

* The request object: 

/:parameters : for ex: `app.get('/api/:thing',...)` and `req.params.thing` OR if its a query string the server itself then `?example=answer` = `req.query.example`

* The response object: it sends data back to the browser and it has methods like: `send()` and `status()` that express uses to format the output to the browser, it also sends headers like cookies and status codes.

## Express Middleware

* It's a series of function that the requests "goes through" and each function of them recieves request, response and next as parameters, and there are two types of middleware: application and route.

* Application Middleware: Error handling, bringing in other routes, JSON parsing and runs on every request.

* Route Middleware: Deals with specific things for route, like "are you logged in?" "what is your IP" "have we seen you here before?"

## Server Testing

* Dont start the actual server for testing, instead export your server as module in a library.

* Then use `supertest` to run tests, this will hit the routes same as running the real tests but without it running.