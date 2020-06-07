# OAuth

## OAUTH 2.0

* OAuth is used in instances like "login with facebook" or "login with github", OAuth is an open standard for access delegation, it grants application access to services without giving a password.

* When you use that, you give them some of your personal information, but they can also (if u agreed to it ) do things like create documents, delete them, or access other services.

## How does OAuth work?

* Its a series of handshakes, the server asks a user if its okay to login as them at a remote service and then begin process of authentication and access

1- site asks for approval 

2- user agrees 

3- remote service contacts the app with one time code 

4- the app calls back to a special address to exchange code for token 

5- if the token is granted, then the app will be able to contact the remote service using that code.

## Access Code

First client needs to grant permission to the app by providing an < a > tag that will take them to service auth page.

## Access Token

User gets redirected with a URI callback with a code, after you provide that code, you can exhange it for an access token my a post request to the auth server and providing information.
