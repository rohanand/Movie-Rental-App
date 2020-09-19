 -> App Deployed on Heroku
 -> MongoDB Databse is hosted on azure cloud on MongoDB Atlas.
Using the API call on postman : 
 -> Users can Signup/Signin
 -> Autharisation/Authentication is done on every signup/signin such that no one can 
 input invalid email id or password and no existing users can again signup .
 -> CRUD operations can be performed after on :
       -> Movies
       -> Genres
       and users can registered on rental service for the movie.
       Here users can post request to create the type of genre they want , movie they want,
       users can get request with the help of authorisation token provided after every signup
       of users with valid email , name and password.
       users can put request to update the details
       users can delete request to delete the type of movie ,genre they want
       users will not be able to see the password as it is encrypted with the help of 'bcrypt'
       package for hashing passwords.
  -> all the validation are done with the help of 'joi' package in npm
  -> Used the Express error middleware to catch any unhandled exceptions in the
    request processing pipeline.
  -> Used express-async-errors package
  -> To log erros , used 'winston' package. Winston can log errors in multiple transports.
    A transport is where the log is stored.
  -> Database used is MongoDb where in the documents , different collections are formed for customer,users,
      genres,movies,rentals.
  -> All my files/codes are unit and integration tested.
       -> unit tested on 'jest' framework
       -> Integration tested on 'supertest'
       
