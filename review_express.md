1) What is middleware, and whats a useful example?

ANSWER***Middleware is code that is executed during communication between a database and an application which allows code to be executed that would normally not otherwise be posssible. A useful example of middleware is express sessions, body parsser

2) What are the HTTP verbs and what's the difference between them?

ANSWER***The most common HTTP verbs or "Mehtods" are GET (Retrievs or 'gets' data from your server), POST (Sends or adds data to your server), PUT (Updates or edits data on your server), & DELETE (Deletes or removes data on your server). 

3) Describe the two patterns of asynchronous functions- callbacks vs async await.

ANSWER***Callbacks: the act of referencing a function within another function, meaning that that function that is enterd as a argument of another function will only execute after the intial function is completed.

ANSWER***Async/Await: code designated with async syntax is meant to run asynchronis while associated code with the await syntax will only execute once the async code has been executed.

4) What is a model and what does it help us do?

ANSWER***A model is a an object with provides structue for a data set ( such as "users).

5) What is session?

ANSWER***Session allows you to temporarily store sensitive data on your server rather then the browser and encryptes the data when passing it back to the browser to be stored in a cookie so that the server can use the encrypted data and associate it back with a specific user

6) I'm getting an error from my template- cannot read 'name' of undefined. What should I check and where?

ANSWER***You should look at the route that is rendering the template, specifcally at the context variable which should be providing the "name" to the template. If there is no issue there, you should also take a look at the model that is providing context to the name property/value.

7) I'm getting an error- "cannot cast to ObjectId for value 'new' at value '_id' for model Review". What the heck does that even mean???

ANSWER***There is a issue with the create route where the query string in the url is not properly tying the req.params.id to the ObjectId.

8) Describe the necessary parts of a form to properly submit to our server. What are some common things to forget or do improperly that will result in bad responses/data?

ANSWER***In order for a form to properly be sumbttimed to our server. You need to insure that the data of the form is wrapped in html form tags in your template as well as provide an action (path) and HTTP method (POST or PUT) as value to the form tag. In your route, the form data will be repersented by "req.body." If you run into issues with form data, my first reccomendation would be to console.log(req.body) in your route that is rendering the tempelate which contains the form data in order to begin the trouble shooting process.

9) Tell your 5 year old cousin how the internet works.

ANSWER***The internet is a global network of connected computers which together help share and distribute information across the network so that all the persons who would like to access that information can do so as long as they have a computer connected to the network.

10) ALGORITHM CHALLENGE: 

In a seperate javascript file, write a LinkedList that works as a priority queue- when you add a new node to the list, it is given a number and finds its spot in line based on that number. Your linkedlist should have the following methods:

add(data, priority)
search(data)
remove() -> remove the head node from the list.
