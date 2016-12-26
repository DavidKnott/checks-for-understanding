## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

<br>
* What is a cookie?
<br>
A cookie stores a string of information on the users client.
<br>
* What’s the difference between a session and a cookie?
<br>
Sessions and cookies are simliar but sessions are more secure.
<br>
* What’s a flash and when do you want to use flashes?
<br>
Flashes are messages that pop up once for the user and go away.  Flashes are best used after the user completes or fails to complete a specific action.
<br>
* Why do people say “HTTP is stateless”?
<br>
HTTP is stateless because the connection between the client and the server is lost with each completed interaction.
<br>
* What’s authentication? Explain.
<br>
Authentication is verifying a users identity, usually with a prevously determined username and password.
<br>
* What’s the difference between authentication and authorization?
<br>
Authentication is finding out who someone is, authorization is determining what they're allowed to access.
<br>
* What’s a before filter?
<br>
Before filters are run before an action in a controller and are usually used to make sure a user is logged in before they are able to view specific content.
<br>
* How do we keep track of a user once they’ve logged in?
<br>
We keep track of a user once they're logged in by storing their user id.
<br>
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
<br>
We want to namspace a resource when we don't need all the functionality of another full resource.  For example namspacing an admin works out well because we only want admins to have slighty more features available to the then normal users.
<br>
* At a high level, what tools can you use to implement authorization? How would you use them?
<br>
We use bcrypt but at a higher level one could use fingerprint scanners and facial recognition.
<br>
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
<br>
An enum allows us to have a set of options such as [default admin].  We store enums in our database as integers and they are declared in our models.
<br>
* What are some strategies you can use to keep your views DRY?
<br>
One can go back over their work and move everything possible from their controllers to their models, then move everything that involves thinking to their controllers.  In general the goal is to push as much proccessing as possible into the models.
<br>
