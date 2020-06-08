# Bearer Authentication


## Overall about bearer tokens 

* Following a signin attemp, by using basic auth (Username and password transmition) or OAuth (handshake/authorization process), the service makes a boolean decision as to the success of the attempt.

* If the signin was successful, it would be more efficient if the server remembered that the client making requests was allowed to.

* Instead of keeping sending username/password or OAuth handshakes, we are able to use an authentication method called Bearer token.

* Bearer tokens are **encoded JSON objects** that contain enough info for the server to assert that any client request have originated from a client that has previously authenticated themselves.

* Upon recieval of the bearer token from a client, a server can decode it, inspect the json object inside and look for appropriate account and re-authenticate the user in a single lookup.

1- Bearer tokens are sent to the client after the initial signin process.

2- Client must make every request to the server with that token in the header.

3- Server checks the token, re-authenticates and grants or denies access.

4- In express it can be done using a middleware.

## JSON Web Tokens

* JWT is a standard that defines a way to securely transmit info between parties as a JSON object.

* This info can be verified and trusted because its digitally signed.

* It can be signed by: 1-Using a secret key 2-Public/Private key pair using RSA or ECDSA.

* When a token is signed using a public/private key, the signature certifies that only the party holding the private key is the one that signed it.

* Signing a token does not secure its content.

## When should you use JSON Web Token

* In Authorization: once the user is logged,each subsequent request will include JWT allowing the user to access routes,services and resources that are permitted with that token.

* SSO (single sign on) is a feature that uses JWT.

* Information Exchange: JWT is a secure way of transmitting info because JWT's can be signed.