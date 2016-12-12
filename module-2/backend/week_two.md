## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
<br>
ActiveRecord seperates the user from sql allowing them to work with sql databases in a more user friendly and readable manner.
<br>
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
<br>
They are class methods because every instance of the class will have the same relationships.
For example all teacher instances will have a has_many relationship with classes and all classes will have a belongs_to 
relationship with a single teacher.
<br>
3. What do they allow you to do?
<br>
They allow us to combine database information allowing for more abstract connections and analysis to be made.
<br>
4. What's the difference between agile workflow and waterfall method?
<br>
Agile is working through planning, testing and executing in small iterations and changing your course on the go.
<br>
Waterfall is trying to do each step (planning, testing and executing, etc) all at once.
<br>
5. What is the difference between `#new` and `#create`?
<br>
New only makes a new instance but doesn't save it.
<br>
Create makes a new instances and saves it.
<br>
6. At a basic level, what does cURL allow you to do?
<br>
It allows us to send http requests from our terminal.
<br>
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
<br>
Assuming we're talking about elementary school, they will have a has_many and belongs_to (many to one) relationship.
<br>
I tried to add a photo for a long time and I couldn't figure out how so I'm going to slack it to you.
<br>
8. Define foreign key, primary key, and schema.
<br>
A foreign key connects the belongs_to with the has_many, in our example it is an attribute of the students table.
<br>
A primary key connects the has_many with the belongs_to, in our example it is an attribute of the teachers table.
<br>
A schema is the blueprint for a database.
<br>
9. Describe the relationship between a foreign key on one table and a primary key on another table.
<br>
Foreign keys link the belongs_to to the primary key on the has_many.
10. What are the parts of an HTTP response?
<br>
Response Header and Response Body.
<br>
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
<br>
Never call classes in the views and make sure to pass everything through the controller so that each part of your Sinatra code is as independent as possible.
<br>


### Optional Questions

<br>
1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
<br>
Where, group, joins, includes, count.
<br>
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
4. What can you expect from a group as you begin working together? As you continue working together?
<br>
I can expect the expectations to be clearly established and as we continue to work together we can continuously refine them.
<br>
5. What two columns does `t.timestamps null: false` create in our database?
<br>
Created_at and updated_at.
<br>
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
<br>
Camel case.
<br>
8. What case does Ruby use for multi-word variables?
<br>
Snake case.
<br>
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
<br>
One to many.
<br>
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
