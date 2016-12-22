## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?
<br>
rails new database=postgresql -T
<br>
2. What do Models generally inherit from in rails?
<br>
They inherit form ActiveRecord::Base
<br>
3. What do Controllers generally inherit from in a rails project?
<br>
They generally inherit from the ApplicationsController
<br>
4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
<br>
get "/horses/:id" to: "horses#show"
<br>
5. What rake task is useful when looking at routes, and what information does it give you?
<br>
Rake routes give the user a list of all existing routes in the terminal.
<br>
6. What is an example of a route helper? When would you use them?
<br>
Route helpers allow the user to create paths without explicitly stating the url e.g. horses_path vs /horses.
<br>
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
<br>
The url is the actual address that will appear for the user while the path is used to navigate the site internally.
<br>
8. What are strong params and why are the necessary?
<br>
Strong params protect the attributes from user assignment, only allowing assignment to take place if they have been listed in strong_params.
<br>
9. What role does `form_for` play in helping us create our forms?
<br>
Form_for is a shortcut that allows us to quickly create forms in rails that usually take in information regarding objects.
<br>
10. How does `form_for` know where to submit the user's input?
<br>
Form_for knows where to submit the users input by looking at where the request to it came from.
<br>
11. Create a form using a `form_for` helper to create a new `Horse`.
<br>
<%= form_for @horse do |f| %>
  <br>
  <%= f.label :name %>
  <%= f.text_field :name %>
  <br>
  <%= f.label :age %>
  <%= f.integer :age %>
  <br>
  <%= f.label :owner %>
  <%= f.string :ownder %>
  <br>
  <%= f.submit %>
<% end %>
<br>
12. Why do we want to validate our models?
<br>
We validate our models to make sure that all the attribute fields are filled in when a user creates a new entry into the database.
<br>
