## Project Setup 

##### Frontend
* [x] BE app is deployed to Heroku
* [x] CI platform is integrated 
* [x] CORS setup in place to enable FE app to call endpoints 

##### Backend
* [x] BE app is deployed to Heroku
* [x] CI platform is integrated 
* [x] CORS setup in place to enable FE app to call endpoints 

## Phase 1/MVP - Sprint 1

##### Home Page
* As an unauthenticated visitor, when I visit the application home page I see a button to view "Needs" and a button to "Create Need"

##### Create
* As an unauthenticated visitor, I can submit a form to create a "Need", with the following attributes:
    * Point of contact [for MVP this is an email address]
    * Description
    * Title
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



## Phase 2 - Sprint 2 (8/31 - 9/8)
* check in ?s: 
  * Balancing cost of data manipulation on FE vs. cost of calls to API with our size of database. Is there a best practice? 
     * Decision: To avoid so many api calls, makes sense to do it on the FE 
     * If we were to scale bigger, we could think about pagination as a way to make it more sustainable to fetch the data on the FE
  * Any flags on direction v1 of signup to lead to an email to the point of contact?
     * Look into doing some kind of library to do this - could help with the secuturity. (Sendgrid, Mailchimp, etc.) 
     * Is there another BE route? have a 'request sent' to BE 
  * Where should we aim to be this week?
     * Aim to have most of the functionality done on Monday 
     * Tuesday for polishing
     * Wednesday code freeze, for demo prep and documentation  

##### Assign category(/ies) to a "Need"
* As an unauthenticated visitor, when I create a "Need," I am prompted to assign <TBD count> cetegory/ies to the need 
   * How are categories created/defined?
      * Hard coded on the BE, including an "other" 
   * How many categories can a user assign?
      * One (for now) in a dropdown menu
         * Maybe build DB to accomodate future iteration with many:many?

##### Filter "Needs Index" page by some attributes
* As an unauthenticated visitor, I can filter the "Needs Index" page by the following attributes:
    * zip-code
    * category
    * start_date

##### "Need Show" page
* As an unauthenticated visitor, I can click on a "Need" from the "Needs Index" to see the details of the need (showing all fields) 
   * This is where full "Description" field is shown (not on index page)  
   
##### Sign up for a "need" 
* Button on the "Need Show" page to sign up to support a "Need"
   * Lead to an email sent to the point of contact
* Remove the need point_of_contact from the Need Index + Need Show page 

## Phase 2B 
* Save the email address of a user when they sign up to support a Need
* Update "Count of supporters needed" on the need index + show
* If we have time: 
   * (hidden link) Organizer view shows all the needs AND the emails of supporters who have signed up 
   
   
## Phase 3 - Sprint 3
##### Create users
* As a visitor to the home page, I have the option to create a user account with a username, email and password
* In this iteration, we'll update the point of contact field on a Need to be a User_ID with a 1:many association 
   
##### Associate users with needs as supporters
* As an authenticated user, I can sign up to support a "Need" that has available supporter slots 
   
##### [TBD] Associate users with needs as points of contact
##### [TBD] Authorization - Assign roles to users (organizer, community member) with different views/permissions
##### [TBD] Authentication - Users can log in

## Feature brain dump - future work 
* Share to social media
* "Organizer" role users can approve/deny "Need" submissions
* User dashboard: On visiting their dashboard, a user can see all upcoming "Needs" they are supporters on, and upcoming "Needs" they are points of contact on. They can also toggle to see past Needs they participated in. 
* Incorporate an add-to-calendar feature when a user signs up to support a "Need"
* Incorporate census data API to show stats about the population of a given zip code on search?
