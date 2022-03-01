# CRUD
### Status Codes Based On REST Methods
In your own words, describe what each group of status code represents:

100’s = **Informational code, lets user know status of loading**
200’s = **Success codes! "hey it's working"**
300’s = **Redirect codes "Hey go to this page now, cuz your page is gone"**
400’s = **Error codes "Uh-oh, something went wrong"**
500’s = **server error codes**
What is a status code 202? **Accepted**
What is a status code 308? **Permanent Redirect**
What code would you use if an update didn’t return data to a client? **404**
What code would you use if a resource used to exist but no longer does?  **308**
What is the ‘Forbidden’ status code?**505**

Why do we need to pull our MongoDB database string out of our server and put it into our .env? **so that it is not pushed up to github**
What is middleware? **software used to mediate between other software.**
What does app.use(express.json()) do?**redirect to server**
What does the /:id mean in a route? **it indicates where it is located in the tree**
What is the difference between PUT and PATCH? **PUT is a method of modifying resource where the client sends data that updates the entire resource . PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.**
How do you make a default value in a schema? **using the default keyword**
What does a 500 error status code mean? **Internal server error**
What is the difference between a status 200 and a status 201? **200=ok 201=created**
