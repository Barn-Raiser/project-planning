## Project Setup 

##### Frontend
* [ ] BE app is deployed to Heroku
* [ ] CI platform is integrated 
* [ ] CORS setup in place to enable FE app to call endpoints 

##### Backend
* [ ] BE app is deployed to Heroku
* [ ] CI platform is integrated 
* [ ] CORS setup in place to enable FE app to call endpoints 

## MVP - Sprint 1

##### Home Page
* As an unauthenticated visitor, when I visit the application home page I see a button to view "Needs" and a button to "Create Need"

##### Create
* As an unauthenticated visitor, I can submit a form to create a "Need", with the following attributes:
    * Point of contact
    * Description
    * Start time
    * End time
    * Address
      * Street Address
      * City
      * State
      * Zip Code   
    * Count of supporters needed
    * Status (to default to active for MVP)
 * The new need will be added to the "Needs" table and will show on the "Needs Index" page
 * Upon submitting a "Need", I will be redirected to the "Needs Index", where I will see the new need listed

##### Index
* As an unauthenticated visitor, I can see the "Needs Index" page which shows all needs, ordered by start date 

## Iteration 2 - Sprint 2
##### Search and filter "Needs" index page by some attributes
* As an unauthenticated visitor, I can filter the "Needs Index" page by <TBD> attributes

##### Assign category(/ies) to a "Need"
* As an unauthenticated visitor, when I create a "Need," I am prompted to assign <TBD count> cetegory/ies to the need 

## Iteration 3 - Sprint 3
##### Create users
* As a visitor to the home page, I have the option to create a user account with a username, email and password
   
##### Associate users with needs as supporters
* As an authenticated user, I can sign up to support a "Need" that has available supporter slots 
   
##### [TBD] Associate users with needs as points of contact
##### [TBD] Authorization - Assign roles to users (organizer, community member) with different views/permissions
##### [TBD] Authentication - Users can log in

## Feature brain dump - future work 
* "Organizer" role users can approve/deny "Need" submissions
* User dashboard: On visiting their dashboard, a user can see all upcoming "Needs" they are supporters on, and upcoming "Needs" they are points of contact on. They can also toggle to see past Needs they participated in. 
* Incorporate an add-to-calendar feature when a user signs up to support a "Need"
* Incorporate census data API to show stats about the population of a given zip code on search?
