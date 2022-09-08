# Readings: CRUD
In your own words, describe what each group of status code represents: 100’s = all is good 200’s = done 300’s = an action is taken. 400’s = a problem 500’s = things are not going as expected

What is a status code 202? the request is accepted ACCEPTED

What is a status code 308? there is a redirect ACCEPTED

What code would you use if an update didn’t return data to a client? 304 not modified

What code would you use if a resource used to exist but no longer does? 410 Gone 301 Moved Permanently

What is the ‘Forbidden’ status code? 403

Why do we need to pull our MongoDB database string out of our server and put it into our .env? <br>
 as .env will stay on our local machine and its not going to be deployed . that will prevent the un Authurized access to database and other resources.

What is middleware? <br>
functions that have access to ( requests, responses), object , and the next middleware function in the application's request-response cycle

What does app.use(express.json()) do? <br>
recognize the incoming Request Object as a JSON Object

What does the /:id mean in a route? 
<br>request params

What is the difference beween PUT and PATCH?

PUT uses request URI to supply a modified version of the requested resource PATCH supplies instructions to modify the resource.

How do you make a defalut value in a schema?

fresh informations

books: {
    type: String,
    default: ''
}
What does a 500 error status code mean?

there is something wrong in the code that being excuted in the server

What is the difference between a status 200 and a status 201?
200 indicates that the request recived and being proccessed . 201 request recived successfully and processed with a successfull result .