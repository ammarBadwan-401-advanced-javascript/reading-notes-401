# Authentication

## User Modeling

* Modern web apps need to model sensitive information because users need to trust that their info won't be leaked.

* Some info like user names, emails and addresses can be saved in plain text if the database is password protected and/or behind a firewall, while other information like passwords should be encrypted using a hashing algorithm before its even stored, this prevents anyone from getting access to a password incuding developers with database permissions.

* User models that have sensitive data should never be sent to client applications.


## Cryptography

* Its a science that studies the methods for encoding messages so that they can be read only by the right person with the required decode info, known as **the key**, it includes cryptanalysis; which is the science of decoding encrypted messages without the key.



## Hash Algorithms

* Cryptographic Hash Algorithm takes piece of data and produces a hard to reverse hash, if identical data is passed into the algortihm the same hash wll always be produced.

* They are usually used to check the integrity of the data.

## Cypher Algorithms

* A Cryptographic Cypher Algorithm takes a piece of data and a key and produces encrypted data which can be reversed into the original data by decrypting it using the same key.

* User seeds get created by a random unique string called **tokenSeed** and then encrypting it with a secret key that only the server knows.


## Basic Authorization

* This is a common method to send username and passwords in an HTTP Request, then they are joined by ":" then "base64 encoded" and placed after the string 'Basic'.

* Server can decode the basic Auth header to retrieve the username and password, if the combination is validated the server responds back to the client with a validation response (token or key) so that the client re-authenticate without continually sending the user/pass.

* In browsers, we use `btoa` to decode and `atob` to decode to/from base64, in node, we use node module to do the same.

