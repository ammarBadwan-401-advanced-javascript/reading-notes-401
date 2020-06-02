# API Server

## Express: Router Parameters

* In express we can read parameters
* We can also run middleware for a specific route if we add it there, or add middleware to all requests if we use app.use().

* With express, you can run a middleware if you want when a specific parameters are present.

## Sub documents in Mongoose

* Mongoose is schema driven object relational mapper (ORM) and this gives us the opportunity to provide structure to our Mongo documents.

* The defaul is non-structured documents in Mongo (and all NoSQL databases), but Mongoose deals with that and provides some level of rules and validation around data models.

* With **Sub Documents** mongoose gives the ability to use schema to describe a deeper part of data model.

* This can be useful for documents that contain other documents.

* Yuo can for example have orders as an array and an array of items and add them as a relation to each other.

* Sub Documents are not “populated” unless you do the above step mangually and its a downside to NoSQL, as it keeps things seperate if you dont do it manually.

## Jonining Data/Documents in Mongo

* NoSQL Databases don't really join and it's considered anti pattern.

* we can use `populate()` in mongoose to connect 2 collections by: 1:physically joining using reference to another colection and 2: by virtual population.

