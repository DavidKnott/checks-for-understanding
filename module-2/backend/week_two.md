## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
ActiveRecord seperates the user from sql allowing them to work with sql databases in a more user friendly and readable manner.
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
They are class methods because every instance of the class will have the same relationships.
For example all teacher instances will have a has_many relationship with classes and all classes will have a belongs_to relationship with a single teacher.
3. What do they allow you to do?
They allow us to combin database information allowing for more abstract connections and analysis to be made.
4. What's the difference between agile workflow and waterfall method?
Agile is working through planning, testing and executing in small iterations and changing your course as you go.
Waterfall is trying to do each step (planning, testing and executing, etc) at once.
5. What is the difference between `#new` and `#create`?
New only makes a new instance but doesnt save it.
Create makes a new instances and saves it.
6. At a basic level, what does cURL allow you to do?
It allows us to send http requests form our terminal.
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
Assuming we're talking about elementary school, they will have a has_many and belongs_to relationship.
![Alt text](file:///Users/Knott/Downloads/Relationship.pdf?raw=true "Optional Title")
8. Define foreign key, primary key, and schema.
9. Describe the relationship between a foreign key on one table and a primary key on another table.
10. What are the parts of an HTTP response?
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
