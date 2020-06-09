# Access Control (ACL)

## Access Controls

* Access controls are the selective restriction of resources, they are impleneted everywhere in computers.

* Websites limit the access to pages based on the user previliges.

* API's restrict access for internal and external developers differently.

* In RESTful API's, its important to limit access based on credentials, this is called Access Control.

## Application Flow and Access Control

* Every application is different and they might give different control levels to different users, but a CMS can:

1- Allow admins to create categories, manage accounts.

2- Allow editors to create,edit and delete existing content but not manage accounts.

3- Allow guests to access content.

4- Allow users (logged in users) to access content and write a comment, but not change the actual content.

* All of those constraints need to be handled by both front and backend of the application stack.

## Back End (API Layer)

* Manage the login cycle with the front end.

* Maintain the user's database.

* Authenticate users (basic and bearer)

* Create, manage and apply role bassed access controls (RBAC)

## Front End (Client Layer)

* Initiate a login process.

* Store login tokens as cookies.

* Manage login state.
