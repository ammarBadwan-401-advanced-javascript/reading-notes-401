# Express Routing

## Routing

* Express routing refers to how an endpoint responds to client requests.

* There are many methods on how to to use the routing, all are derived from the HTTP methods, these methods include:

1- GET method route, ex: `app.get('/', function (req, res) {res.send('GET request to the homepage')})`.

2- POST method route, ex: `app.post('/', function (req, res) {res.send('POST request to the homepage')})`.

You can define the route itself and the callback function after it (req,res) and then respond to it whichever way you see fit.

You can also use middleware callback functions using `app.use()`.

* Express 4.0 comes with a new Router that provides us with routing api's like `.use , .get , .param etc...`

* We can get the value of a unique route like `/:name` by using the params middleware that exists within express itself.