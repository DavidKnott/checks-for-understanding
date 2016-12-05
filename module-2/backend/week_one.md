## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
GET - Sends a page and can be used to input information.
POST - Recieves information from user.
PUT - Used to update information.
PATCH - Also used to updatea information.
DELETE - Used to delete information.
2. What is Sinatra?
Sinatra is a framework that facilitates buildding webpages.
4. What is MVC?
Model, View, Controller
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
We follow conventions to prepare us for rails, so that other developers will understand us andbecause we want the tools we use to understand us.
6. What types of variables are accessible in our view templates without explicitly passing them?
Instance variables.
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @counter = 1
    erb :index, :locals => {:name => "Mr. Ed"}
  end
  ```
@counter = 1

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
 :locals => {:name => "Mr. Ed"}
9. What's the purpose of ERB?
ERB allows us to output ruby to a webpage.
10. Why do I need a development AND test database?
If we only add one database it would be constantly changing from testing and we would be constantly cleaning it and remaking it which would be very slow if we used the data from the development database.
11. What's responsive design?
Responsive design changes the layout of a web page to match the users screen size.
12. What is CRUD and why is it important?
Create
Read
Update
Delete
It's important because it allows us to modify a database in the 4 most critical ways.
13. What does HTTP stand for?
Hyper Text Transfer Protocol.
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
<% "ruby" %>
<%= "ruby" %>
The one with the equals outputs the other one thinks.
15. What's an ORM?
Object relational mapping.
16. What's the most commonly used ORM?
SQL.
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
get '/restaurants'
get '/restaurants/:id'
get '/restaurants/:id/edit'
get '/restaurants/new'
Delete '/restaurants/:id'
Put '/restaurants/:id'
Post '/resturants'

18. What's a migration? 
Migration makes the schema.
19. When you create a migration, does it automatically modify your database?
Yes, it sets up the database to recieve information.
20. How does a model relate to a database?
A model houses the classes through which the database can be accessed, i.e. Trip class has trips database.  The classes also contain analysis, relations, and validations.
21. What's the difference between agile workflow and waterfall method?
The Waterfall method is doing each step once (i.e . plan, test, execute) and then hoping that the final product works how you want it to.
Tee Agile method is all about planing, testing, and executing in small chunks and then doing it again many times while contanstly making minor adjustments to your course each time.
22. What is the difference between `#new` and `#create`?
When we use new it doesn't save the info into our database, create does.
